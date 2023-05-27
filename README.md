# Syslog synthetic log generator
A synthetic syslog log generator that can be used for sending test data to ZincObserve. 

## Prerequisites

1. A ZincObserve server running that is running and has has its port 5514 accessible (Not blocked by a firewall or something else).
1. Syslog logging enabled on the ZincObserve server. See [docs](https://zinc.dev/docs/guide/ingestion/logs/syslog/) for more details.
1. The IP address / subnet is authorized on the ZincObserve server.


## Testing

Start a terminal and run the following command


```shell
python syslog_gen.py --host <ZincObserver host> --port 5514 --file sample_logs.txt --count 100000
```

e.g.

```shell
python syslog_gen.py --host 127.0.0.1 --port 5514 --file sample_logs.txt --count 100000
```


