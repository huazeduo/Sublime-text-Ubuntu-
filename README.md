# Sublime-text在Ubuntu下创建启动器和桌面快捷方式 
 在Ubuntu下使用sublime_text3作为文本编辑器，与gedit使用相同的方式直接在控制台编辑文本、
 1、安装 sublime_text3
 下载地址https://www.sublimetext.com/  下载对应系统的版本  安装成功后配置启动项。
 2、在桌面创建快键方式。
    在Desktop创建文件sublime.desktop，内容如下：
    创建成功后保存，赋予sublime.desktop权限，chmod 777 sublime.desktop
    
    [Desktop Entry]
    Name=Sublime Text 2
    Comment=Sublime Text 2
    Exec=/home/huazd/Downloads/sublime_text_3/sublime_text  //安装路径
    Icon=/home/huazd/Downloads/sublime_text_3/Icon/48x48/sublime-text.png //图标路径
    Terminal=false
    Type=Application
    Categories=Application;Development;
    StartupNotify=true

在命令行下启动：
创建一个软连接即可
sudo ln -s  /home/huazd/Downloads/sublime_text_3/sublime_text /usr/bin/sublime 

在控制台输入sublime add.cc，相比于gedit和vim更好用一点 
huazd@ubuntu:~/Documents/c/c++primer/1$ sublime add.cc 



    





    


    

