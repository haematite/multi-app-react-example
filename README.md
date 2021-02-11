# multi app example

[react-advanced-configuration](https://create-react-app.dev/docs/advanced-configuration/)

# build

```bash
yarn --cwd root-app/ run build
mkdir _build/
cp -t _build -v -a -f -- root-app/build/*

yarn --cwd p1-app/ run build
mkdir _build/p1
cp -t _build/p1 -v -a -f -- p1-app/build/*

yarn --cwd p2-app/ run build
mkdir _build/p2
cp -t _build/p2 -v -a -f -- p2-app/build/*
```

# serve

```bash
python3 -m http.server -d _build/
```
