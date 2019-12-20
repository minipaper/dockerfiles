FROM node:12.14.0-alpine

# Install smi2srt
RUN npm install -g smi2srt

VOLUME ["/opt/smi"]

ENTRYPOINT ["smi2srt", "-n", "/opt/smi"]
