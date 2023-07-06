# Somaesthete's k8s resources and notes.

## Ingest

.. ingest these raw docker commands into k8s manifests.

#### Runs an LX instance specific to growplate.

    docker run -p 26901:6901 -p 3030:3030/udp nargetdev/novnc-plantilx:v0.0.0 /home/headless/eclipse-workspace/plantiLX/runWherever.sh


#### Runs a webrtc streaming server (serves up realtime USB stream )

    docker run -d --device=/dev/video0 --device=/dev/video1 -p 8000:8000 -it mpromonet/webrtc-streamer
