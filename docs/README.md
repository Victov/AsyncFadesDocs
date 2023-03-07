# Simple Async Fades Documentation

This page contains user documentation for the (Simple Async Fades)(TODO:Link) plugin.

This plugin adds 4 asynchronous blueprint nodes into UE5. These nodes can be used to easily fade the screen, without having to keep track of fading logic yourself. The nodes have several output pins that fire at the end of a fading operation, or during a dip (also known as fade out, do something, fade in).

### Fade
![fadeasync](./images/FadeAsync.png "Fade Async Node")
![fadecolorasync](./images/FadeColorAsync.png "Fade Color Async Node")

### Dip
![dipasync](./images/DipAsync.png "Dip Async Node")
![dipcolorasync](./images/DipColorAsync.png "Dip Color Async Node")

### Feature comparison

| **Node/Features**    | **Behaviour**                                               | **Color**      | **Tick while paused** | **Split-screen supported** | **Affected by Time Dilation** |
|----------------------|-------------------------------------------------------------|----------------|-----------------------|----------------------------|-------------------------------|
| **Fade Async**       | Fade between Game and Black                                 | Black          | No                    | No                         | Yes                           |
| **Fade Color Async** | Fade between Game and Color                                 | User specified | No                    | No                         | Yes                           |
| **Dip Async**        | Fade from Game to Black, perform action, fade back to Game. | Black          | No                    | No                         | Yes                           |
| **Dip Color Async**  | Fade from Game to Color, perform action, fade back to Game. | User specified | No                    | No                         | Yes                           |


