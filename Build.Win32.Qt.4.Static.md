e.g. we have source code under: 

    H:\Qt\qt-everywhere-opensource-src-5.4.0
    /h/Qt/qt-everywhere-opensource-src-5.4.0
    export QtSCD="/h/Qt/qt-everywhere-opensource-src-5.4.0"
    
then

  1. cd $QtSCD
  2. sed -i -e "s|QMAKE_LFLAGS = .*|QMAKE_LFLAGS = -static -static-libgcc -static-libstdc++|g" "mkspecs/win32-g++/qmake.conf"