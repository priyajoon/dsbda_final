# dsbda_final
-> start-all.sh
-> export hcp=$(hadoop classpath)
-> javac -cp ${hcp} *.java
-> jar -cvf my.jar *.class
-> hadoop fs -mkdir /input
-> hadoop fs -put input.txt /input
-> hadoop jar my.jar WordCount /input /output
-> hadoop fs -cat /output/*
-> stop-all.sh 
