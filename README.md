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
$ zip -r release/electron-react-app-linux-armv7l.zip release/electron-react-app-linux-armv7l/
$ scp release/electron-react-app-linux-armv7l.zip pi@raspberrypi.local:/home/pi/

# connect raspberry pi
$ ssh pi@raspberrypi.local
$ unzip electron-react-app-linux-armv7l.zip
$ cd electron-react-app-linux-armv7l
$ chmod +x electron-react-app
$ DISPLAY=:0 ./electron-react-app
```
