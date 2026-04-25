# Install k9s in Ubuntu VM

**Note:** Do not use snap install. Use the Ubuntu's native package manager dpkg.

## Install k9s

### 1. Download the latest official .deb package

```bash
wget https://github.com/derailed/k9s/releases/latest/download/k9s_linux_amd64.deb
```

### 2. Install it using native package manager

```bash
sudo dpkg -i k9s_linux_amd64.deb
```

### 3. Cleanup the downloaded file

```bash
rm k9s_linux_amd64.deb
```

### 4. Access k9s

```bash
k9s
```
**You should see the k9s terminal interface**

## Microk8s config

**k9s looks for `~/.kube/config` . If this is not created, you will see an empty cluster on k9s. Makesure you run the following command, so that the config file is available.**

```bash
microk8s config > ~/.kube/config
```

## Apply Custom Themes

### 1. Check Config and Skins Paths using;

```bash
k9s info
```
### 2. Add the customt theme YAML file in Skins

```bash
vim /home/boffinuser/.config/k9s/skins/tokyonight.yaml
```

### 3. Edit Config and include skin under ui.skin

```yaml
  ui:
    skin: tokyonight
```








