### Development

Install latest nodejs

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.0/install.sh | bash
source ~/.bashrc
nvm install v22.15.0
```

Install pnpm:

```
npm install -g pnpm
```

Install packages:

```
pnpm install
```

Run

```
pnpm run dev
```

build packages

```
cd packages

for dir in */; do
  echo "$dir"
  cd "$dir"
  pnpm build
  cd ..  
done
```

installed svelte-gravatar:

```
cd apps/app && pnpm install svelte-gravatar && pnpm install svelte-file-dropzone
```

