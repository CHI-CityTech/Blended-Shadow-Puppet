# Lumbra: The Ancient Game of Light and Shadow
![DALL·E 2024-11-16 16 25 48 - Lumbra the Game woodcut](https://github.com/user-attachments/assets/6df3691c-8009-4b87-89e4-5fe59eb40027)

Lumbra is an ancient strategic game rooted in the metaphors of light and shadow. Played on a square grid board, the game combines elements of illumination, concealment, and reflection to outmaneuver the opponent. The goal is to dominate the board by harnessing light or shadow.

---

## **Objective**

- The **Light** side seeks to illuminate the board, controlling the majority of tiles through light.
- The **Shadow** side aims to cast the board into shadow, controlling the majority of tiles through darkness.
- Victory is achieved through **Territorial Control**, **Piece Capture**, or **Zone Domination**.

---

## **Game Setup**

### Board
- The game board begins with a predefined configuration of light and shadow.
- It is a a square grid, typically 8x8 or 10x10. 
- **Stationary Light Emitters**:
  - Positioned at the four corners or edges of the board.
  - Emit fixed beams of light in specific directions, creating illuminated tiles and casting shadows.
  - These emitters are not movable and are considered part of the board itself.
- **Initial Light and Shadow Zones**:
  - Tiles affected by stationary emitters start illuminated.
  - Tiles not hit by stationary emitters’ light beams start in shadow.
  - the number of different lights that hit a square determine the intensity of it's lightness
### **Pieces**
  - Each piece has unique abilities and interactions with light and shadow.
  - Each piece is designed to emit, block or modify the light sources, using flames, opaque, transluscent reflective and other types of mechanisms. The result is that differetn squares or piedces are illuminated or cast into shadow based on the moves made by the players.
  - Pieces are placed in starting positions based on the chosen board setup or scenario.
  - Often gameplay begins as each person places one of their pieces onto teh board, similar to the way that Go is played
  - Each side has their own specific pieces with their own mechanics.

   - **Light Side**:
     - Emitters
     - Mirrors
     - Prisms
     - Guardians
   - **Shadow Side**:
     - Blockers
     - Veils
     - Shadow Candles
     - Creepers
---

## **Gameplay**

### **Turn Structure**

Each player performs one action per turn:
- **Move** a piece to a new tile.
- **Rotate** a piece to change its orientation.
- **Activate/Extinguish** a piece’s light or shadow ability.

---

### **Capture Mechanics**

1. **Shadow Pieces**:
   - A shadow piece is removed from the board if it is no longer within a shadow zone at the end of a turn.

2. **Light Pieces**:
   - A light piece is removed from the board if it is no longer illuminated by a light source at the end of a turn.

---

### **Light and Shadow Dynamics**

1. **Light Beams**:
   - Travel in straight lines until blocked.
   - Illuminate all tiles in their path.

2. **Shadows**:
   - Created directly behind blockers relative to light sources.
   - Block illuminated tiles, returning them to neutral or shadowed states.

3. **Reflections**:
   - Mirrors and reflective tiles redirect beams to new paths.

4. **Shadow Amplification**:
   - Shadow Candles extend shadow zones to adjacent tiles.

---

## **Specific Pieces and Their Abilities**

### **Light Side Pieces**
1. [**Emitter**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Light-Emitter.md)
   - **Ability**: Projects a straight beam of light.
   - **Weakness**: Can only emit light in one direction; easily blocked.

2. [**Mirror**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Light-Mirror.md)
   - **Ability**: Redirects light to illuminate hard-to-reach tiles.
   - **Weakness**: Stationary and vulnerable if surrounded.

3. [**Prism**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Light-Prism.md)
   - **Ability**: Splits a light beam into two or three paths.
   - **Weakness**: Does not emit light on its own; relies on other pieces.

4. [**Guardian**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Light-Prism.md)
   - **Ability**: Moves freely while illuminating adjacent tiles.
   - **Weakness**: Limited illumination range.

---

### **Shadow Side Pieces**
1. [**Blocker**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Shadow-Blocker.md)
   - **Ability**: Casts a wide shadow behind it based on orientation.
   - **Weakness**: Vulnerable if rotated incorrectly.

2. [**Veil**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Shadow-Veil.md)
   - **Ability**: Creates a zone of total shadow, nullifying light in adjacent tiles.
   - **Weakness**: Cannot move once placed.

3. [**Shadow-Candle**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Shadow-Candle.md)
   - **Ability**: Emits dim light that strengthens nearby shadows.
   - **Weakness**: Stationary and limited in range.

4. [**Creeper**](https://github.com/CHI-CityTech/Blended-Shadow-Puppet/blob/main/CLane/Lumbra/rules/pieces/Shadow-Creeper.md)
   - **Ability**: Extends shadows as it moves, enveloping tiles in darkness.
   - **Weakness**: Cannot block beams directly.


# Lumbra Game Pieces Summary Table

## **Light Team**

| **Piece**           | **Movement**             | **Abilities**                                                                                                   | **Capture Conditions**                                |
|----------------------|--------------------------|----------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| **Emitter**          | Rotates freely; immobile | Emits a focused light beam; interacts with Prisms and Mirrors to extend or redirect light beams                | Removed if no longer illuminated by any light source |
| **Prism**            | 1 tile orthogonally/diagonally | Splits light into multiple beams; redirects light at various angles                                            | Removed if surrounded by shadow                      |
| **Mirror**           | 1 tile orthogonally/diagonally | Redirects light based on the angle of incidence; supports one-sided and two-sided variants                     | Removed if surrounded by shadow                      |
| **Guardian**         | Immobile                 | Projects a protective light aura; shields nearby tiles and Light pieces from Shadow influence                  | Removed if surrounded by shadow                      |

---

## **Shadow Team**

| **Piece**           | **Movement**             | **Abilities**                                                                                                   | **Capture Conditions**                                |
|----------------------|--------------------------|----------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| **Blocker**          | 2 tiles orthogonally     | Casts shadows to block light beams; amplifies shadows when near Shadow Candles                                 | Removed if not in a shadow zone                      |
| **Shadow Candle**    | 1 tile orthogonally/diagonally | Extends and amplifies shadows; casts dim light to enhance nearby Shadow pieces                                 | Removed if fully illuminated                         |
| **Creeper**          | 2 tiles orthogonally/diagonally | Infiltrates illuminated zones; disables Guardians; leaves temporary shadow trails                              | Removed if exposed to 2+ light beams simultaneously  |
| **Veil**             | 1 tile orthogonally/diagonally | Generates an aura of enhanced darkness; amplifies nearby shadows; dampens light intensity                      | Removed if fully illuminated                         |

---

## **Neutral Pieces**

| **Piece**                      | **Movement** | **Abilities**                                                                                                   | **Capture Conditions**                                |
|---------------------------------|--------------|----------------------------------------------------------------------------------------------------------------|------------------------------------------------------|
| **Stationary Light Emitters**   | Immobile     | Provides consistent illumination across specific board areas; interacts with Prisms and Mirrors                | Not capturable                                       |
| **Stationary Shadow Absorbers** | Immobile     | Potential ability to nullify shadows within a specific radius; details pending game mechanic discussions        | Not capturable                                       |

---

**Notes**:
- Pieces are grouped into **Light**, **Shadow**, and **Neutral** categories for clarity.
- Neutral pieces are features of the board and not controlled by either side but interact with gameplay mechanics.
- Capture Conditions outline what leads to the removal of Light and Shadow pieces; Neutral pieces are fixed features and cannot be removed.

**Return to [Game Pieces Index](#)**



---

## **Victory Conditions**

1. **Territorial Control**:
   - Control the majority of tiles (illuminated or shadowed) by the end of the game.

2. **Piece Capture**:
   - Remove the opponent’s critical pieces (e.g., Emitters or Blockers).

3. **Zone Domination**:
   - Illuminate or shadow specific key tiles for a designated number of turns.

---

## **Sample Gameplay**

1. **Turn 1**:
   - Light Player places an Emitter, projecting a beam across four tiles.
   - Shadow Player places a Blocker, casting a shadow over the beam’s path.

2. **Turn 2**:
   - Light Player uses a Prism to split the beam and bypass the shadow.
   - Shadow Player rotates a Shadow Candle to strengthen the shadow zone.

3. **Turn 3**:
   - Light Player illuminates a sacred tile for control.
   - Shadow Player moves a Veil to nullify the light on the sacred tile.

---

**Enjoy the Game of Lumbra!**
