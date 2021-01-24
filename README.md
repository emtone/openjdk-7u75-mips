# openjdk-7u75-mips
Port from openjdk-7u75-src-b13-18_dec_2014 for mips

# Build Tips:
1 set ALT_BOOTDIR and ALT_OUTPUTDIR path  
ALT_BOOTDIR=xxx  
ALT_OUTPUTDIR=xxx  
export ALT_BOOTDIR ALT_OUTPUTDIR  
  
2 corba not support mips  
export BUILD_CORBA=false  
  
3 unset JAVA_HOME and CLASSPATH  
unset JAVA_HOME  
unset CLASSPATH  
  
4 build command  
make 2>&1 | tee $ALT_OUTPUTDIR/build.log  
