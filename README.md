# AExOp-DCS

## Algorithm to explore and Optimiza Descriptor Configuration Spaces

### Requirements

Java 1.8

### Usage

~~~
java -jar AExOp-DCS.jar --help

usage: cmd [-a <arg>] [-c <arg>] [-e <arg>] [-h] [-i] [-p <arg>] [-s
<arg>] [-v]

-a,--arch <arg>       SERIAL for a serial execution or MULTICORE for a
parallel execution

-c,--csvfile <arg>    output, path to csv file

-e,--endpoint <arg>   property target

-d,--debug            create logs folder for save application logs

-h,--help             Show this help and exit

-i,--info             print project configuration

-p,--project <arg>    path to project file .qproj

-s,--sdffile <arg>    input, path to sdf file

-v,--version          show the version and exit
~~~

### Example
~~~
java -jar AExOp-DCS.jar.jar -p proj_25D_100MD.qtproj -s ace_COR3D_training.sdf -c subset.csv -e Activity -d
~~~

After start the execution, two folders will create: generated_descriptors and logs. 

- generated_descriptors will have the list of each computed and considered MD for every family.
- logs folder is created if -d option is set.  
