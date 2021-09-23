# rnw-64-bundle-bug-repro
Repro of an issue I'm experiencing with RNW 0.64.18

## Steps

1. git clone https://github.com/luisnaranjo733/rnw-64-bundle-bug-repro.git
1. npm install
2. npm start
3. Click green play button in Visual Studio, Debug | x64 config targeting Local Machine

Steps I used to create this repro (nothing special)
```
npx react-native init rnw64test --template react-native-template-typescript@6.6.* --npm --title RNW64Test
cd rnw64test
npx react-native-windows-init --overwrite
```

## Expected result

App launches and loads

## Actual result

App launches but never loads

## Screenshot 
Notice that metro bundler thinks the bundle is loaded, but the UI never shows up in the app
![Screenshot of repro](/screenshot.png)