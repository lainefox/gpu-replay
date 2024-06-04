# GPU Replay

## Installation
1. Install `gpu-screen-recorder` from your distro's package manager
2. git clone this repo and navigate into the folder
   ```bash
   git clone https://github.com/lainefox/gpu-replay && cd gpu-replay
   ```
3. Copy `gpu-replay` to `/usr/local/bin`
   ```bash
   cp gpu-replay /usr/local/bin/
   ```
4. Copy `gpu-replay.service` to `~/.config/systemd/user`
   ```bash
   cp gpu-replay.service ~/.config/systemd/user/
   ```
5. (Optional) If you want the service to start with the system run
   ```bash
   systemctl --user enable gpu-replay
   ```

## Usage
### Starting gpu-replay
Start the SystemD service
```bash
systemctl --user start gpu-replay
```

**OR**

Run the script with the start argument (the script will take over the shell you are running it in)
```bash
gpu-replay start
```
### Saving a replay
Run the script with the save argument
```bash
gpu-replay save
```
### Stopping gpu-replay
Stop the SystemD service
```bash
systemctl --user stop gpu-replay
```

**OR**

Run the script with the start argument in a shell
```bash
gpu-replay stop
```
