1、window安装MinGW :https://nuwen.net/mingw.html#install
2、common文件夹中 gcc -c mongoose.c
3、http_client文件夹中：g++ -c http_client.cpp ;g++ -c main.cpp
4、把common中生成的mongoose.o拷贝到http_client 文件夹中
5、g++ -o main *.o -lws2_32   //-lws2_32很重要，因为moogoose.c是在vc中编译的，不加这个用MinGW编译会报错。
6、服务器中同意的方法进行编译
