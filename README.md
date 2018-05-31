## Pre-requisites
To start, you need to get a MapR 6.0.0 running. You can install your own cluster or download a sandbox.

### Step 1: Create the stream

A *stream* is a collection of topics that you can manage together for security, default number or partitions, and time to leave for the messages.

Run the following command on your MapR cluster:

```
$ maprcli stream create -path /user/ranjitlingaiah/sample-stream
$ maprcli stream edit -path /user/ranjitlingaiah/sample-stream -produceperm p -consumeperm p -topicperm p