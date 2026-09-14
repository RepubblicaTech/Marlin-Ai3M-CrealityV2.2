# Backstory

If you read the description, your question would be:
> Why this weird combo?

Well, long story short: i broke my Anicubic i3 Mega board and I needed a replacement quick.
Since we had a unused Creality CR10-S5, I took its external case and decided to use it as a replacement board.

The hardware part was kind of easy, the only modification were to invert a few of the cables that connect the motors and to adapt wires like the nozzle thermistor to a JST connector out of the "proprietary" cable that was directly connected to a custom Anycubic PCB. 

On the firmware side, i started from the defualt config for the CrealityV2.2 board and changed essential settings like print sizes. I also noticed one of the onboard MOSFET for the bed heater was likely shorted out so the board was giving constant "heat up" signals to the bed, so i had to change the pins to D11 (i chose that place). Which also meant creating a connector for that part.

# What next?

For now, the board still sits in that Creality case, but i don't want the actual mess that I currently have, so I may print various "adapters" sooner or later to screw the Creality board into the Anycubic casing, remove all unnecessary cables (and re-do the cable management).

# To be honest...

...I didn't do all of this by myself. I have to say i went back-and-forth with Google Gemini to get most of the help, especially regarding the firmware configuration since Marlin has A LOT of settings to go through.
But still, this was a nice thing spending some time on.

Probably nobody will ever need something like this, but at least I can keep it somewhere safe for the time being. Or i guess if you ever want to mod your Anycubic printer and use a Creality board, then you're welcome.

# NOTES

I may or may not try keeping this fork as updated as i can to the upstream project.