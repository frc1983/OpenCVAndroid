# OpenCVAndroid
Projeto baseado no exemplo de face detection e na implementacao de Roman Hošek.


Devem ser baixados: 
  - OpenCV4Android SDK: http://sourceforge.net/projects/opencvlibrary/files/opencv-android/
  - Android NDK: https://developer.android.com/ndk/downloads/index.html

Deve ser ajustado:
  - Arquivo local.properties do projeto Android.
    - Adicionar a linha apontando para o local do NDK descompactado:  Ex.: ndk.dir=C\:\\android-ndk-r10e 
  - Arquivo Android.mk na pasta jni do projeto Android.
    - Ajustar o local do SDK do OpenCV: Ex.:  OPENCV_CAMERA_MODULES:=on
                                              OPENCV_INSTALL_MODULES:=on
                                              #OPENCV_LIB_TYPE:=STATIC
                                              include D:/OpenCV-android-sdk/sdk/native/jni/OpenCV.mk
  - Arquivo Application.mk na pasta jni do projeto Android.
    - Colocar a versão da arquitetura utilizada: Ex.: APP_ABI := armeabi-v7a
    


