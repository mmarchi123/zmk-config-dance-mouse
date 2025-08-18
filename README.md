# Dance! Split Keyboard with Cirque Trackpad

## Cirque Trackpad Integration

### Pin Connections

The Cirque trackpad connects to the Nice!Nano v2 using the following pin mappings:

#### SPI Connections
| Cirque Pin    | Nice!Nano Pin | Notes           |
|---------------|---------------|-----------------|
| SCK (Clock)   | D3           | P0.20          |
| MOSI          | D7           | P0.11          |
| MISO          | D4           | P0.22          |
| CS            | D8           | Chip Select     |
| DR            | D9           | Data Ready      |

#### Power Connections
| Cirque Pin    | Nice!Nano Pin |
|---------------|---------------|
| VCC           | 3.3V         |
| GND           | GND          |

### Important Installation Notes

⚠️ **Critical Setup Requirements**:

1. **Power Supply**
   - The trackpad must be powered with 3.3V
   - Use the 3.3V pin from the Nice!Nano exclusively

2. **Wiring Best Practices**
   - Keep SPI wires (SCK, MOSI, MISO) as short as possible
   - Use proper shielding if available
   - Maintain signal integrity by avoiding long or unshielded cables

3. **Installation Checklist**
   - ✓ Verify all connections are secure and well-soldered
   - ✓ Double-check for shorts between pins
   - ✓ Ensure proper pin alignment during connection
   - ✓ Test continuity before powering up

4. **Troubleshooting**
   - Verify voltage at the VCC pin is 3.3V
   - Check for cold solder joints
   - Ensure no pins are bridged or shorted
   - Verify SPI pins are correctly mapped in firmware

# My config for [dance!](https://github.com/chase-hunter/dance)

# Features
- Mouse keys
- Dongle [prospector](https://github.com/carrefinho/prospector-zmk-module) 

## keymap
![dance! Keymap](keymap_img/dance_keymap.svg)

Here are the pin connections between the Cirque trackpad and the Nice!Nano v2, based on your current configuration in dance_right.overlay:

SPI Connections:
SCK (Clock) → D3 (P0.20)
MOSI → D7 (P0.11)
MISO → D4 (P0.22)
CS (Chip Select) → D8 (pro_micro 8)
DR (Data Ready) → D9 (pro_micro 9)
Power Connections:
VCC → 3.3V
GND → GND
Here's a visual representation:

Important notes:

The trackpad operates on 3.3V - make sure to use the 3.3V pin from the Nice!Nano
Keep the SPI wires (SCK, MOSI, MISO) as short as possible to ensure reliable communication
Make sure the connections are secure and well-soldered
Double-check that none of these connections are shorting with each other or with other pins

lambda time?
