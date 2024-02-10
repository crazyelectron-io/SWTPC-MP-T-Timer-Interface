# SWTPC MP-T Timer Interface

The MP-T Interrupt Timer is a 5 1/4 inch x 3 1/2 inch circuit board implemented with the 5009 programmable counter/ divider and 6820 peripheral interface adapter integrated circuits.

## Overview

The board provides software selectable interrupts of 1 usec, 10 usec, 100 usec, 1 msec, 10 msec, 20 msec, 100 msec, 1 sec, 10 sec, 100 sec, 1 min, 10 min or 1 hour.
Since only half of the 6820 peripheral interface adapter is used for the interrupt timer the other half has been fully buffered to provide a general purpose eight bit input port along with one buffered "data read" input line and one buffered "data accepted" output line for complete handshake control.
The interface is completely software programmable by the user with interrupt control as well as polarity control of the input port handshake lines.

> Introduced by Southwest Technical Products Corporation in 1976.
> The MP-T kit cost $40.

## Custom parts library

This repository uses a custom parts repository as submodule.
Use the command `git submodule add https://github.com/crazyelectron-io/KiCAD_custom_parts.git library/custom_parts` once in the root of the project (after initial creation).
When later committing the FD-2 repository, the submodule dependency is also registered and when cloning it again, run the following commands to get the submodule(s) back:

```bash
git submodule init
git submodule update
```

To use the updated libraries after a custom part is added or updated, just run `git submodule update` to retrieve the changed libraries.
