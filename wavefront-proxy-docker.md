docker run \
   -e WAVEFRONT_URL=https://longboard.wavefront.com/api/ \
   -e WAVEFRONT_TOKEN=xxx \
   -e JAVA_HEAP_USAGE=512m \
   -e WAVEFRONT_PROXY_ARGS="--otlpGrpcListenerPorts 30001" \
   -p 2878:2878 \
   -p 30001:30001 \
   wavefronthq/proxy:latest
