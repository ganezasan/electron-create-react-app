# Electron create react application

## install
```
yarn install
```
## run append

```
yarn run electron
```

## build & package for raspberry pi

After run package, please check release folder.
```
$ yarn run build
$ yarn run package
```

## run app on raspberry pi

```
$ zip -r release/hoge-linux-armv7l.zip release/hoge-linux-armv7l/
$ scp release/hoge-linux-armv7l.zip pi@raspberrypi.local:/home/pi/

# connect raspberry pi
$ ssh pi@raspberrypi.local
$ unzip hoge-linux-armv7l.zip
$ cd hoge-linux-armv7l
$ chmod +x hoge
$ DISPLAY=:0 ./hoge
```
