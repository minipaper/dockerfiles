Convert subtitles in ".smi" or ".ass" format to ".srt" format.

# Usage

In Windows Command Line (cmd)
```shell script
docker run --rm -v %cd%:/data minipaper/smi2srt
```

In PowerShell, you use ${PWD}
```shell script
docker run --rm -v ${pwd}:/data minipaper/smi2srt
```

On Linux:
```shell script
docker run --rm -v $(pwd):/data minipaper/smi2srt
```

# create an alias
```shell script
# for linux
$ alias smi2srt='docker run --rm -u $(id -u):$(id -g) -v $(pwd):/data minipaper/smi2srt-dl'

# for windows 10 cmd
# https://gist.github.com/minipaper/8ed450f5a2869e13c5d345b01476eed0
doskey smi2srt=docker run --rm -v %cd%:/data minipaper/smi2srt $*
```


# Reference
https://github.com/axfree/smi2srt
