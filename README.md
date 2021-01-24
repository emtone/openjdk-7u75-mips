# openjdk-7u75-mips
Port from openjdk-7u75-src-b13-18_dec_2014 for mips

Build Tips:
# set ALT_BOOTDIR and ALT_OUTPUTDIR path
ALT_BOOTDIR=
ALT_OUTPUTDIR=
export ALT_BOOTDIR ALT_OUTPUTDIR
# corba not support mips
export BUILD_CORBA=false
# unset JAVA_HOME and CLASSPATH
unset JAVA_HOME
unset CLASSPATH
# build command
make 2>&1 | tee $ALT_OUTPUTDIR/build.log
