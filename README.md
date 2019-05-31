Description
===========
movie thumbnailer (mtn)  
fork from http://moviethumbnail.sourceforge.net/  

Movie Thumbnailer (mtn) saves thumbnails (screenshots) of movie or video files to image files (jpg, png).
It uses FFmpeg's libavcodec as its engine, so it supports all popular codecs, e.g. h.265/hevc, h.264, mpeg1, mpeg2, mp4, vc1, wmv, xvid, divx...     
mtn was originaly developed by tuit (tuitfun); though most of its magic is actually done
by FFmpeg libraries. For documents, please see in the doc directory and at
https://gitlab.com/movie_thumbnailer/mtn/wikis/home .


Dependency
==========
 - ffmpeg   (>=3.1)
 - gd       (>=2.0.35)

Getting source
==============
```
$ git clone https://gitlab.com/movie_thumbnailer/mtn.git
$ cd mtn/src
```

Installing from source
======================

**[Fedora](https://getfedora.org/)** 26
```
$ dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm
$ dnf install ffmpeg-devel gd-devel make gcc-c++  
$ make
$ sudo make install
```

**[Debian](https://www.debian.org/)** 9, **[Ubuntu](https://www.ubuntu.com/)** 17.10, **[LinuxMint](https://linuxmint.com)** 19, **[MX Linux](https://mxlinux.org/)** 18, ...  
```
$ sudo apt-get install libgd-dev libavutil-dev libavcodec-dev libavformat-dev libswscale-dev make  
$ make
$ sudo make install
```

**[Archlinux](https://www.archlinux.org/), [Manjaro](https://manjaro.org/)**  

Movie Thumbnailer is available in AUR as [mtn-git](https://aur.archlinux.org/packages/mtn-git)

**[OpenSUSE](http://opensuse.org/)** 15  
(FFmpeg in repository is unfortunately compiled with only a few video codecs)
```
$ zypper install ffmpeg-4-libavcodec-devel ffmpeg-4-libavdevice-devel ffmpeg-4-libavformat-devel ffmpeg-4-libswscale-devel gd-devel freetype2-devel libjpeg62-devel make gcc 
$ make
$ sudo make install
```

**[CentOS](https://centos.org/)** 7  
```
$ yum localinstall https://download1.rpmfusion.org/free/el/rpmfusion-free-release-7.noarch.rpm    
$ yum install ffmpeg-devel gd-devel make gcc-c++    
$ make  
$ sudo make install  
```

**[FreeBSD](https://www.freebsd.org/)** 10  
```
$ pkg install gmake ffmpeg libgd
$ gmake
```

**Windows**  
```
C:\..\mtn\src> Make.MinGW.bat
```

**macOS [(brew)](https://brew.sh/)** 10.14.2 (1.8.6)
```
$ brew install ffmpeg libgd
$ make
$ sudo make install
```

References
==========
 * [FFmpeg project](http://www.ffmpeg.org)
 * [libgd project](https://libgd.github.io)
 * [libgd library and dependecies](http://gnuwin32.sourceforge.net/packages/gd.htm)
 * [MinGW](http://www.mingw.org/)
 * [RPM Fusion repository](https://rpmfusion.org/)
 * [RPM Macros](https://docs.fedoraproject.org/en-US/packaging-guidelines/RPMMacros/)
 * [GitLab yaml](https://docs.gitlab.com/ee/ci/yaml/README.html)
