<img width="79" height="43" alt="image" src="https://github.com/user-attachments/assets/42aff6df-4b18-4d8f-ba0d-1a58b6c22c70" /># your_team_name

Hello! This is a template repository in which you can upload your deliverables for the CHORAS ASSA Workshop. The deliverables are

1. 🎧 Impulse response from DE (.wav)

2. 📊 T30 results from DE in (.csv)

3. 5️⃣ Frequencies of first 5 modes from DG in (.csv)

4. (Optional) 📊 T30 results from DG (up to the 250Hz band) in (.csv) as calculated with pyfar

5. 📃 This readme filled with the correct information :)

_Feel free to remove this section when you're done :)_

## Members

- Tim
- Judith

## Process

This is where you can describe how you tackled the task

- First we forked and cloned CHORAS and set up the app via the link of [localhost] (http://localhost:5173/)
- Then we forked and cloned the ASSA_Workshop repository. This geometry file could be imported into CHORAS webapp.
- We entered the source and receiver positions.
- We assigned materials to surfaces.
- We entered the simulation settings
- etc.

## Input settings

For reproducibility of your results we would like to know what inputs you used to complete your simulations.


Diffusion Equation method
- Simulation length: EDT
- Impulse response length: 0.5 s
- Speed of sound: 343 m/s
- Energy decay threshold: 35 dB
- Characteristic length (m): 3

Discontinuous Galerkin method
- We duplicated the simulation
- 


### Geometry

Room2215_simple

### Source position

- x:4.5
- y:3
- z:1.5

### Receiver position

- x:4
- y:4.5
- z:1.2

### Surfaces

If you created materials you can list them here with their absorption coefficients:

- _material name_: 63 Hz, 125 Hz, 250 Hz, 500 Hz, 1000 Hz, 2000 Hz, 4000 Hz

    _Example:_

- My new material, 0.1, 0.2, 0.3, 0.4, 0.5, 0.1, 0.1

Material properties:

- Surface [1]: _material name_
- Surface [6]: _material name_
- Rest of the surfaces: _material name_

### Settings

You can paste the JSON here by clicking on the Open as JSON button in the Settings tab.

- DE

```json
<DE settings as JSON>
```

- DG

```json
<DG settings as JSON>
```

## 3 proposals for improving CHORAS

Here you can list your 3 proposals for improving CHORAS. Out of the box ideas are welcome!

- Proposal 1: Make clear the which axes are which. For example, when you hover over an axis, you see that it is the x-axis.
- Proposal 2: Simulation length could use some more information.
- Proposal 3: The tab says "app" with a lightning icon. Can you make it your own logo?
- Proposal 4: The export of the "parameters_simulation_1.csv" does not include the frequency bands.

## Functionality issues

Please list any functionality issues you found:

- Issue 1: When positioning the source/receiver the value can sometimes shoot back to the previous value.
- Issue 2
- ...

## Feedback / experience

Below you can tell us your feedback or describe your experience of working with CHORAS today! Please start every bullet with **I like..** or **I wish/wonder..**

- I like ..
- I wish ..
- I wonder ..
- ..
