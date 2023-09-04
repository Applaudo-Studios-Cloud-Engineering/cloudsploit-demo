## Cloudsploit Demo

# Build CLI (Buildpack)

Install Pack CLI

```bash
sudo add-apt-repository ppa:cncf-buildpacks/pack-cli
sudo apt-get update
sudo apt-get install pack-cli
```

[Reference](https://buildpacks.io/docs/tools/pack/)

Build Container

```bash
git clone git@github.com:Applaudo-Studios-Cloud-Engineering/cloudsploit-demo.git
cd cloudsploit-demo
git submodule update --init
cd cloudsploit
pack build cloudsploit --buildpack paketo-buildpacks/nodejs   --builder paketobuildpacks/builder:base
```

# Runninc CLI

```
docker run cloudsploit --help
```

