### Crate Folder
```
mkdir -Folder-Name-
cd -Folder-Name-
```

### Start Node Project With TypeScript

```
npm init -y
npm install typescript --save-dev
npm install @types/node --save-dev
```

### Create a tsconfig.json

```
npx tsc --init --rootDir src --outDir build \
--esModuleInterop --resolveJsonModule --lib es6 \
--module commonjs --allowJs true --noImplicitAny true
```

### Remove the content of tsconfig.json to
```
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "lib": ["es6"],
    "allowJs": true,
    "outDir": "build",
    "rootDir": "src",
    "strict": true,
    "noImplicitAny": true,
    "esModuleInterop": true,
    "resolveJsonModule": true
  }
}
```

### Create File
```
mkdir src
touch src/index.ts
```

### Compiling our TypeScript
npx tsc

### Run The Project
```
node .\dist\index.js
```

### Create Executable
```
pkg installation
npm i pkg
```

### Create Package
```
pkg dist\index.js --targets node12-win-x64
```
