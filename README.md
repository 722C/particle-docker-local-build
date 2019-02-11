This is a customized Docker image based off of [makercrew/particle_build](https://hub.docker.com/r/makercrew/particle_build/) for the purposes of building [Particle's Device OS](https://github.com/particle-iot/device-os) locally without having to obtain all of the correct dependency versions.

### Example

```bash
docker run -ti --rm --workdir="/particle_src/main" -v ~/Desktop/device-os/:/particle_src 722c/particle-docker-local-build /bin/bash -c "make PLATFORM=boron MODULAR=n APP=../tests/app/ble/scanner all program-dfu"
```
