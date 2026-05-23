# Graph Report - .  (2026-05-21)

## Corpus Check
- Corpus is ~17,778 words - fits in a single context window. You may not need a graph.

## Summary
- 337 nodes · 402 edges · 19 communities detected
- Extraction: 93% EXTRACTED · 7% INFERRED · 0% AMBIGUOUS · INFERRED: 28 edges (avg confidence: 0.76)
- Token cost: 100 input · 100 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]
- [[_COMMUNITY_Community 3|Community 3]]
- [[_COMMUNITY_Community 4|Community 4]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_Community 6|Community 6]]
- [[_COMMUNITY_Community 7|Community 7]]
- [[_COMMUNITY_Community 8|Community 8]]
- [[_COMMUNITY_Community 9|Community 9]]
- [[_COMMUNITY_Community 10|Community 10]]
- [[_COMMUNITY_Community 11|Community 11]]
- [[_COMMUNITY_Community 12|Community 12]]
- [[_COMMUNITY_Community 13|Community 13]]
- [[_COMMUNITY_Community 14|Community 14]]
- [[_COMMUNITY_Community 15|Community 15]]
- [[_COMMUNITY_Community 16|Community 16]]
- [[_COMMUNITY_Community 19|Community 19]]
- [[_COMMUNITY_Community 20|Community 20]]

## God Nodes (most connected - your core abstractions)
1. `AcEnv` - 18 edges
2. `colorize()` - 15 edges
3. `Logger` - 13 edges
4. `SacAgent` - 10 edges
5. `EpisodeLogger` - 10 edges
6. `ACSocket` - 9 edges
7. `proc_id()` - 8 edges
8. `ReplayBuffer` - 7 edges
9. `get_delta_to_car_ahead()` - 6 edges
10. `get_delta_to_car_behind()` - 6 edges

## Surprising Connections (you probably didn't know these)
- `AcEnv` --uses--> `ACSocket`  [INFERRED]
  standalone/sac/ac_environment.py → standalone/ac_socket.py
- `main()` --calls--> `AcEnv`  [INFERRED]
  standalone/main.py → standalone/sac/ac_environment.py
- `main()` --calls--> `SacAgent`  [INFERRED]
  standalone/main.py → standalone/sac/sac.py
- `AcEnv` --uses--> `ACController`  [INFERRED]
  standalone/sac/ac_environment.py → standalone/ac_controller.py
- `main()` --calls--> `ACSocket`  [INFERRED]
  standalone/main.py → standalone/ac_socket.py

## Communities (21 total, 4 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.06
Nodes (28): format_time(), get_car_in_pit_lane(), get_delta_to_car_ahead(), get_delta_to_car_behind(), get_drs_enabled(), get_fuel(), get_gear(), get_location() (+20 more)

### Community 1 - "Community 1"
Cohesion: 0.07
Nodes (20): AcEnv, Extra information returned by step and reset functions., A reward considering just speed., The custom gymnasium environment for the Assetto Corsa game., A reward considering speed and progress on track., A reward just considering delta progress on track., A reward considering speed and delta progress on track., A reward considering speed, angle and distance from center of track.         :r (+12 more)

### Community 2 - "Community 2"
Cohesion: 0.06
Nodes (16): get_car_name(), get_cars_count(), get_driver_name(), get_session_status(), get_session_type(), get_track_config(), get_track_length(), get_track_name() (+8 more)

### Community 3 - "Community 3"
Cohesion: 0.08
Nodes (18): A simple FIFO experience replay buffer for SAC agents., # TODO: Fix this, Initialize a replay buffer., Compute the Q-losses for the Q-networks.         :param data: The data to use f, Compute the pi loss for the policy.         :param data: The data to use for th, Perform a single update of the SAC model.         :param data: The data to use, Get an action from the actor-critic.         :param observation: The observatio, Perform SAC training on the environment. (+10 more)

### Community 4 - "Community 4"
Cohesion: 0.08
Nodes (19): Logger, Some simple logging functionality, inspired by rllab's logging.  Logs to a tab, Print a colorized message to stdout., Log a value of some diagnostic.          Call this only once for each diagnost, Log an experiment configuration.          Call this once at the top of your ex, Save the data from a driving episode to a JSON file., Load an experiment configuration from a saved JSON file.          This functio, Saves the state of an experiment.          To be clear: this is about saving * (+11 more)

### Community 5 - "Community 5"
Cohesion: 0.11
Nodes (20): format_time(), get_best_lap_time(), get_current_lap_time(), get_invalid(), get_lap_count(), get_lap_delta(), get_laps(), get_last_lap_time() (+12 more)

### Community 6 - "Community 6"
Cohesion: 0.09
Nodes (10): get_brake_temp(), get_tyre_dirty(), get_tyre_pressure(), get_tyre_temp(), get_tyre_wear_value(), Retrieve tyre wear of a tyre. 100 is mint condition, 0 is fully worn (puncture), Retrieve "dirty level" or a tyre. 0 is clean, 5 is most dirty     :param tyre:, Retrieve temperature of a tyre in a location     :param tyre: int [0,3]     :p (+2 more)

### Community 7 - "Community 7"
Cohesion: 0.14
Nodes (12): Render the environment; a PyGame renderer is not needed for AC., ACSocket, Set up the socket connection.         :param host: The host to connect to (defa, Wait for an incoming connection and return the socket object., Send a message to the client to request data, and then receive the data., Send an empty message to the client so it knows training has been completed., Ensure socket is properly closed before terminating program., Socket connection with the Assetto Corsa app.     This is used to get real-time (+4 more)

### Community 8 - "Community 8"
Cohesion: 0.14
Nodes (13): combined_shape(), count_vars(), mlp(), MLPActorCritic, MLPQFunction, Helper functions that combines shape and length., Actor-critic network that contains a policy and two Q-functions., Helper function that creates a multi-layer perceptron. (+5 more)

### Community 9 - "Community 9"
Cohesion: 0.17
Nodes (15): acMain(), acShutdown(), acUpdate(), connect(), The shutdown function of the app, called on app close., The function called when the start button is pressed.     :param args: The argu, The function called when the training has stopped.     :param args: The argumen, Attempts to connect to the socket server. (+7 more)

### Community 10 - "Community 10"
Cohesion: 0.21
Nodes (11): allreduce(), mpi_avg(), mpi_fork(), mpi_op(), mpi_statistics_scalar(), mpi_sum(), num_procs(), Count active MPI processes. (+3 more)

### Community 11 - "Community 11"
Cohesion: 0.15
Nodes (12): abs_level(), get_has_drs(), get_has_ers(), get_has_kers(), get_max_fuel(), get_max_rpm(), Retrieves whether car driven by player has DRS     :return: 0 if no DRS, 1 if t, Retrieves whether car driven by player has ERS     :return: 0 if no ERS, 1 if t (+4 more)

### Community 12 - "Community 12"
Cohesion: 0.2
Nodes (8): get_brake_input(), get_clutch(), get_gas_input(), get_steer_input(), Retrieve the gas input given to a car     :param car: the car selected (user is, Retrieve the brake input given to a car     :param car: the car selected (user, Retrieve the clutch status in the game of a car     :param car: the car selecte, Retrieve the steering input given to a car     :param car: the car selected (us

### Community 13 - "Community 13"
Cohesion: 0.29
Nodes (4): SimInfo, SPageFileGraphic, SPageFilePhysics, SPageFileStatic

### Community 14 - "Community 14"
Cohesion: 0.39
Nodes (7): get_all_datasets(), get_datasets(), main(), make_plots(), plot_data(), For every entry in all_logdirs,         1) check if the entry is a real directo, Recursively look through logdir for output files produced by     spinup.logx.Lo

## Knowledge Gaps
- **127 isolated node(s):** `The main function of the app, called on app start.     :param ac_version: The v`, `The update function of the app, called every frame.     :param deltaT: The time`, `The shutdown function of the app, called on app close.`, `The function called when the start button is pressed.     :param args: The argu`, `The function called when the training has stopped.     :param args: The argumen` (+122 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `colorize()` connect `Community 7` to `Community 1`, `Community 3`, `Community 4`?**
  _High betweenness centrality (0.070) - this node is a cross-community bridge._
- **Why does `AcEnv` connect `Community 1` to `Community 7`?**
  _High betweenness centrality (0.053) - this node is a cross-community bridge._
- **Why does `EpisodeLogger` connect `Community 3` to `Community 4`?**
  _High betweenness centrality (0.034) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `AcEnv` (e.g. with `ACController` and `ACSocket`) actually correct?**
  _`AcEnv` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 9 inferred relationships involving `colorize()` (e.g. with `.__init__()` and `.connect()`) actually correct?**
  _`colorize()` has 9 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `SacAgent` (e.g. with `EpisodeLogger` and `main()`) actually correct?**
  _`SacAgent` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 3 inferred relationships involving `EpisodeLogger` (e.g. with `ReplayBuffer` and `SacAgent`) actually correct?**
  _`EpisodeLogger` has 3 INFERRED edges - model-reasoned connections that need verification._