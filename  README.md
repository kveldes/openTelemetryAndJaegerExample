# Jaeger Example

This is a simple example that demonstrates how to use the OpenTelemetry SDK to instrument a simple application and export to a Jaeger backend.It is a modified example of the original example found in the following link: (https://github.com/open-telemetry/opentelemetry-java-docs/tree/main/jaeger)

# How to run
Prerequisites

    -Java 1.8+
    -Docker 19.03
    -Jaeger 1.16 - Link

1 - Run Jaeger

```
docker run --rm -it --name jaeger\
  -e COLLECTOR_OTLP_ENABLED=true \
  -p 4317:4317 \
  -p 16686:16686 \
  jaegertracing/all-in-one:1.39
  
```

2 - Start the Application from your favorite IDE.

3 - Open the Jaeger UI

Navigate to:

```
http://localhost:16686

```