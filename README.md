# MikuPiano

###### 这是一个基于C++14编写的钢琴游戏.它使用了SFML引擎.
###### resources文件中包含了36个钢琴键的音频文件以及一个单独的arial.ttf字体文件.
###### 我在考虑这个程序的时候,我发现从C3-B5的一共36个琴键,正好可以用10个数字键+26个字母键来表示,所以钢琴音键到键盘的映射关系就是按照这个思路做的.
###### 在windows 上使用 winlib gcc 结合 cmake 构建的命令为:
```shell
cd Piano

mkdir build
cd build

cmake -G "MinGW Makefiles" -DCMAKE_C_COMPILER=gcc -DCMAKE_CXX_COMPILER=g++ ..
mingw32-make -j 4
```
========================================================================================
###### Using C++ to build a virtual piano program.
###### This program is build with SFML engine and C++14. 
###### The resources files contains 36 piano keys and 1 arial.ttf font file.
###### When I design this program, I found that, 26 letters + 10 digits is 36, just fit for our need with keyboard. So I chose C3 -> B5 for this.
###### Just enjoy it!
###### The project uses winlib gcc, build with cmake:
```shell
cd Piano

mkdir build
cd build

cmake -G "MinGW Makefiles" -DCMAKE_C_COMPILER=gcc -DCMAKE_CXX_COMPILER=g++ ..
mingw32-make -j 4
```

![image](https://github.com/yuanluo2/MikuPiano/assets/49439486/fb50057f-d293-4be6-9cf6-d0128e1bdd15)

