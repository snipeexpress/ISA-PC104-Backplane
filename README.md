This project was something I decided to build based on those backplanes you find on ebay or Aliexpress.
to spice it up, I decided to add a couple items from other projects I liked such as the CPU activity indicator from Sergey Kiselev's 8-bit ISA backplane
as well as the option rom socket found here:
https://www.alexandrugroza.ro/microelectronics/system-design/isa-backplane/index.html
Another idea I had was that I wanted to be able to have different modules to play with on it that would use the PC104 socket so you could use a PC104 video card, sound card or other items like that.
I made an adapter board for the ICOP SOM304RD-VI: 
https://www.icop.com.tw/product/SOM304RD-VI
Which on final testing, works as intended. this essentially is a way for me to develop hardware for different devices to be consolidated down later into smaller footprints similar to the TinyLlama by Eivind Bohler,
or the WeeCee by Rasteri. This gives me access to the full ISA bus as well as the ability to change out the device acting as the "compute" 

The first version worked but required a significant amount of bodges to fix some oversights but I wanted to add termination resistors to the last ISA slot and the 
ATX screw holes were slightly off. I also wanted to make the traces to the ISA slots a bit thicker for signal quality.
The second version corrected these issues from version one however, I decided it was a good idea to add a POST card on the board. the thought here is that 
whether you're using a PC104 motherboard or an ISA motherboard, you will be able to get a POST readout without having to add an additional card.
Version 2 had some issues as well since I let a lot of feature creep happen with different ideas I had. the version that is currently posted fixes these issues.

I wouldn't suggest building this one as is just yet, at least not until I correct a few other issues.
If I can't get the POST card to work properly as is then I may either scrap it, change the design completely or even possibly build a PC104 version of it.
Standby for future updates.
