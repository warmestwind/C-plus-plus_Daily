Reference:  
http://wolfprojects.altervista.org/articles/dll-in-c-for-python  
https://www.cnblogs.com/woshitianma/p/3681745.html  


In this folder, I generate a __dll.dll__ by __func.cpp__ and __func.h__.  
__(1)__ Then the __call_dll.py__ can utilize __ctypes__ module to call this dll.  
__(2)__ If you want to load this dll for c plus plus , you need configurate you project attribute page as follow:  
          VC++ -> Include -> path/to/__func.h__  
          VC++ -> Lib -> path/to/__dll.lib__  
          Linker -> Input -> Additional dependency -> __dll.lib__  
        In addtion, you need add __dll.dll__ to the folder of __call_dll.exe__.  
