# cog-pyannote

## Useful commands

```
nvidia-smi
htop
docker exec sd cat predict.log
```

`cog build -t speaker-diarization`
We need to use --network="host" so that docker can access localhost where mini_httpd serves up a local data directory.
`docker run -d -p 5000:5000 --add-host host.docker.internal:host-gateway --gpus all speaker-diarization`