# Tools

### setup_vscode

```sh
code --install-extension esbenp.prettier-vscode
code --install-extension zongou.simple-runner
```

### get:cr

```sh
cd /tmp
if ! test -d cr; then
  git clone https://github.com/zongou/cr
fi
cd cr
cargo run build:release
cargo run install
```

### get:fresh

```sh
VERSION=$(curl -s -S "https://api.github.com/repos/sinelaw/fresh/releases" | jq -r .[0].tag_name)
echo "Downloading fresh-editor ${VERSION}"
ARCH=$(uname -m)
URL=https://github.com/sinelaw/fresh/releases/download/v0.4.6/fresh-editor-${ARCH}-unknown-linux-musl.tar.gz
curl -L ${URL} | gzip -d | tar -C /usr/local/bin --strip-components=1 -x --wildcards "*/fresh"
fresh --version
```

### get:helix

```sh
VERSION=$(curl -s -S https://api.github.com/repos/helix-editor/helix/releases | jq -r .[0].tag_name)
echo "Downloading helix editor ${VERSION}"
ARCH=$(uname -m)
URL=https://github.com/helix-editor/helix/releases/download/${VERSION}/helix-${VERSION}-${ARCH}-linux.tar.xz
curl -L ${URL} | xz -d | tar -C /usr/local/bin --strip-components=1 -x --wildcards "*/hx"
ln -snf /opt/helix-${VERSION}-${ARCH}-linux/hx /usr/local/bin/hx
hx --version
```

### get:dufs

```sh
VERSION=$(curl -s -S https://api.github.com/repos/sigoden/dufs/releases | jq -r .[0].tag_name)
echo "Downloading dufs ${VERSION}"
ARCH=$(uname -m)
URL=https://github.com/sigoden/dufs/releases/download/${VERSION}/dufs-${VERSION}-${ARCH}-unknown-linux-musl.tar.gz
curl -L ${URL} | gzip -d | tar -C /usr/local/bin -x
dufs --version
```

### get:trzsz

```sh
VERSION=$(curl -s -S https://api.github.com/repos/ruanimal/trzsz-rs/releases | jq -r .[0].tag_name)
echo "Downloading trzsz ${VERSION}"
ARCH=$(uname -m)
URL=https://github.com/ruanimal/trzsz-rs/releases/download/${VERSION}/trzsz-${VERSION}-${ARCH}-unknown-linux-musl.tar.gz
curl -LkSs "${URL}" | gzip -d | tar -C /usr/local/bin -x
trzsz --version
```

### get:ttyd

```sh
VERSION=$(curl -s -S https://api.github.com/repos/zongou/ttyd/releases | jq -r .[0].tag_name)
echo "Downloading ttyd ${VERSION}"
ARCH=$(uname -m)
URL=https://github.com/zongou/ttyd/releases/download/${VERSION}/ttyd.${ARCH}
curl -LkSs "${URL}" > ttyd
chmod +x ttyd
sudo mv ttyd /usr/local/bin
ttyd --version
```

### get:cloudflared

```sh
VERSION=$(curl -s -S https://api.github.com/repos/cloudflare/cloudflared/releases | jq -r .[0].tag_name)
echo "Downloading cloudflared ${VERSION}"
URL=https://github.com/cloudflare/cloudflared/releases/download/${VERSION}/cloudflared-linux-amd64
curl -LkSs "${URL}" > cloudflared
chmod +x cloudflared
sudo mv cloudflared /usr/local/bin
cloudflared --version
```
