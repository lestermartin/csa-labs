# Word Count Exercise

This exercise is the "Hello, World!" of Flink exercises.  It will demonstrate how to submit a Flink job.  The Flink job
will read a stream of data from a port, count the use of each word in the stream, and write the result to stdout.

## Exercise Prerequisites

1. This exercise requires *two* terminals with the following working directory:

    ```shell
    $ cd ~/training_materials/csa-labs/flink-exercises/wordcount
    ```
   
2. Build and package the Flink job as a jar file:

    ```shell
    mvn clean package
    ```
   
## Use netcat to send data to a port

In one of the terminal windows, type the following command:

```shell
nc -l 9999
```

Next, type some words into the terminal, for example:

```shell
Hello World
```

Note: You should leave the terminal open and the ```nc``` command running.  You will use the terminal again to add additional 
words to the stream.

