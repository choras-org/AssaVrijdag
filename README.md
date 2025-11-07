<img width="11.58" height="11.85" alt="image" src="https://github.com/choras-org/AssaVrijdag/blob/main/aucustic.webp" />

# Judith & Tim

## Process

This is where you can describe how you tackled the task

- First we forked and cloned CHORAS and set up the app via the link of [localhost] (http://localhost:5173/)
- Then we forked and cloned the ASSA_Workshop repository. This geometry file could be imported into CHORAS webapp.
- We entered the source and receiver positions.
- We assigned materials to surfaces.
- We entered the simulation settings
- etc.

## Input settings
Diffusion Equation method
- Simulation length: EDT
- Impulse response length: 0.5 s
- Speed of sound: 343 m/s
- Energy decay threshold: 35 dB
- Characteristic length (m): 3

Discontinuous Galerkin method
- We duplicated the simulation
- Freq upper limit
- Air density: 1.214 kg/m^3

### Geometry

Room2215_simple

### Source position

- x:10
- y:6
- z:1.5

### Receiver position

- x:3
- y:4.5
- z:1.2

### Surfaces

If you created materials you can list them here with their absorption coefficients:

- _material name_: 63 Hz, 125 Hz, 250 Hz, 500 Hz, 1000 Hz, 2000 Hz, 4000 Hz

- My new material, 0.1, 0.2, 0.3, 0.4, 0.5, 0.1, 0.1

Material properties:

- Surface [1]: wood
- Surface [2-7]: single pane glass
- Surface [8]: wood
- Surface [9-11]: pile and felted wood rug
- Surface [12]: acoustic ceiling (rockwool)
- Surface [13]: corfloor tiles


### Settings

You can paste the JSON here by clicking on the Open as JSON button in the Settings tab.

- DE

```json
{
  "sim_len_type": "edt",
  "de_ir_length": 0.5,
  "de_c0": 343,
  "edt": 35,
  "de_lc": 3
}
```

- DG

```json
<DG settings as JSON>
```
## T30 DE and DG
|Freq [Hz] |	DE T30 [s] | DG T30 [s]|
|-----     |-----        |----|
| 31,5     |-            | 0,434 |
|63        |-            | 0,692 |
|125	     |1.23         | 0,925 |	
|250	     |0.89         | -     |
|500       |0.69         | -     |
|1000      |0.59         | -     |
|2000      |0.52         | -     |


## Room Modes
- 35 HZ
- 46 Hz
- 62 Hz
- 77 Hz
- 99 Hz

## 3 proposals for improving CHORAS
- Proposal 1: Make clear the which axes are which. For example, when you hover over an axis, you see that it is the x-axis.
- Proposal 2: Simulation length could use some more information.
- Proposal 3: The tab says "app" with a lightning icon. Can you make it your own logo?
- Proposal 4: The export of the "parameters_simulation_1.csv" does not include the frequency bands.
- Proposal 5: Choose the third octave bands in the results as well.

## Functionality issues
- Issue 1: When positioning the source/receiver the value can sometimes shoot back to the previous value.
- Issue 2
- ...

## Feedback / experience

Below you can tell us your feedback or describe your experience of working with CHORAS today! Please start every bullet with **I like..** or **I wish/wonder..**

- I like ..
- I wish ..
- I wonder ..
- ..
