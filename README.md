# Syslog synthetic log generator

A synthetic syslog log generator that can be used for sending test data to OpenObserve.

## Prerequisites

1. A OpenObserve server running that is running and has has its port 5514 accessible (Not blocked by a firewall or something else).
1. Syslog logging enabled on the OpenObserve server. See [docs](https://openobserve.ai/docs/ingestion/logs/syslog/) for more details.
1. The IP address / subnet is authorized on the OpenObserve server.

## Testing

Start a terminal and run the following command

```shell
python syslog_gen.py --host <OpenObserve host> --port 5514 --file sample_logs.txt --count 1000
```

e.g.

```shell
python syslog_gen.py --host 127.0.0.1 --port 5514 --file sample_logs.txt --count 1000
```
