# Wumpus_Agent_Game_webApp
logic flows in agent moves!<br>
This implements an intelligent knowledge-based agent that navigates the Wumpus World environment using propositional logic and resolution refutation. The agent perceives its surroundings (breeze and stench), maintains a knowledge base (KB), and uses logical inference to deduce safe cells before moving.<br>
**KEY FEATURES**<br>
- Dynamic Grid Sizing: 2x2 to 6x6, user adjustable
- Random Hazard Placement: Wumpus, pits (15% chance), and gold placed randomly each game
- Percept System: Breeze near pits, Stench near Wumpus
- Resolution Refutation Engine: Proves cell safety using CNF and clause resolution
- Color-Coded Grid: Green (safe), Blue (visited), Gray (unknown)
- Real-Time Metrics: Moves, inferences, position, percepts
- Event Log: Complete history of agent decisions
<br>**Resolution Refutation**<br>
To prove a cell is safe (~P_r_c AND ~W_r_c):<br>
- Negate the goal (assume P_r_c is true)
- Convert KB + negated goal to CNF
- Resolve clause pairs looking for contradiction
- Empty clause = contradiction = goal proven true
<br>**Requirements**<br>
- Any modern web browser (Chrome, Firefox, Edge, Safari)
- No server or internet connection needed
<br>**Setup**<br>
- Save the HTML code as wumpus.html
- Double-click to open in browser
- Game starts automatically

