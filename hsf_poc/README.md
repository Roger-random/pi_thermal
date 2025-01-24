# Heat Sink Fan Proof of Concept

This CadQuery project explores the idea of dissipating heat from the back
side of a Raspberry Pi. This is a less efficient heat path, compared to the
standard practice of pulling heat directly from the top of the CPU, but the
lower efficiency can be made up with brute force: we have more room on the
back to attach a bigger thermal solution.

What's a beefy thermal solution readily at hand for electronics tinkerers?
The CPU heaat sink fan assembly from a desktop PC. Specifically, the stock
Intel cooler for processors on the LGA1150 socket. 4th Gen Core (Haswell)
and 5th Gen Core (Broadwell).

The central adapter has four standoffs spaced for M2.5 screws to secure a
Raspberry Pi. It also has four holes for the stock Intel HSF to clip into
the plate. Between the Pi and the Intel cooler is an aluminum slug turned
on a metalworking lathe. Thermal pads are placed between the aluminum
slug and the bottom of the Raspberry Pi to fill in gap ranging 1-3mm
depending on components soldered to the bottom of the Pi. Thermal paste
fills the thin void between the slug and the Intel CPU cooler.

The adapter is supported by a stand to give the fan a little extra room to
pull in air. This turned out to be unnecessary. The Intel cooler is designed
to dissipate 60-80W of heat. The ~5-10W of a Raspberry Pi under full load
can be dissipated completely passively by the aluminum+copper assembly,
no fan required.
