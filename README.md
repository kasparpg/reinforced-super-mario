# 🎮 Super Mario Advance 2 - NEAT AI

Train an AI to play Super Mario Advance 2 using **NEAT (NeuroEvolution of Augmenting Topologies)** - the same algorithm behind the famous [MarI/O](https://www.youtube.com/watch?v=qv6UVOQ0F44) video!

## Why NEAT?

- **No keyboard hijacking** - Runs headless, you can use your computer normally
- **Evolves network topology** - Automatically discovers the right neural network structure
- **No gradients needed** - Works great with sparse rewards like platformers
- **Visual feedback** - MarI/O-style visualization showing inputs, outputs, and controller

## Quick Start

1. **Install dependencies:**
   ```bash
   pip install neat-python numpy opencv-python matplotlib pillow
   ```

2. **Add your ROM:**
   Place `Super Mario Advance 2.gba` in the `data/` folder

3. **Run the notebook:**
   Open `main.ipynb` and run all cells

## Features

- 🧬 **NEAT Evolution** - Evolves both weights AND network structure
- 💾 **Auto-save** - Best genome saved automatically when fitness improves
- 📊 **Training visualization** - Fitness graphs and statistics
- 🎮 **MarI/O-style playback** - Watch the AI play with input visualization
- 🧠 **Network visualization** - See the evolved neural network topology

## Project Structure

```
├── main.ipynb          # Main training notebook
├── neat-config.txt     # NEAT algorithm configuration
├── data/
│   └── Super Mario Advance 2.gba
└── models/
    ├── best_genome.pkl       # Auto-saved best genome
    ├── winner_genome.pkl     # Final winner after training
    └── neat-checkpoint-*     # Training checkpoints
```

## Configuration

Edit `neat-config.txt` to tune the evolution:
- `pop_size` - Population size (default: 50)
- `fitness_threshold` - Target fitness to stop training
- `conn_add_prob` / `node_add_prob` - Mutation rates for network growth

## License

For educational purposes only. You must provide your own legally obtained ROM.
