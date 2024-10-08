https://huggingface.co/datasets/sidovic/LearningQ-qg

# Description
| Field       | Annotation                 | Example                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ----------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| context     | the text of the passage    | the diode is our first semi-conductor device , and it 's a really important one . every other semi-conductor is basically made from combinations of diodes . and here 's a picture of a diode that you can buy . this is a , just a small little glass package , and that distance right there is about four millimeters . and inside here , right inside here , is a little silicon chip , and it 's manufactured to be a diode . so the question is , what is a diode ? a diode is something that conducts current in one direction , and does not conduct current in the other direction . and the symbol we use for a diode looks like this . it has this big arrow here , that points in the direction of the forward current . one way to understand how a diode works is to draw an iv curve for it . so let 's draw an iv curve for a diode . if it was a perfect diode , made in some unknown technology , what would happen is in the reverse direction , if the voltage across the diode was negative , we 'll label the voltage this way , if the voltage across the diode was negative , that is , this terminal is at a higher voltage than this terminal , there would be zero current flowing . and then for any positive voltage , basically the diode would look like a wire . so i can call that , that 's essentially model number zero of a diode . now when we build real diodes , what happens is we do n't quite get that perfect behavior , so in particular , if we build a diode out of silicon , we can go to a , i 'll go to a number one model . and a silicon diode actually does n't conduct to a slight positive voltage , and then it would go up like that , where this is around point six volts . for a lot of simple circuits that we build , this is a pretty good iv model of a diode . just as a reminder , when we have the iv curve of resistors , a resistors iv curve looks something like this , it was a line that went through zero , and had a constant slope , so a diode is a really different kind of device , it 's a non-linear device , as we can see from this . let me move up here and now we 'll go to a next level model , that is actually the one i wan na talk about most . this is the model of diode that we use most of the time , so i 'll call this model number two . this is the model that you use when you 'll simulate circuits or simulate diodes and we 're gon na talk about this a little bit more . when you have a diode , if i gave you a diode like this , and i said what 's the iv curve of it ? so what i would do is i would find some sort of box that made voltage for me , a power supply , with an adjustment on it , and then i would also have something that read current . so this is an ammeter , and this is a voltage supply . and we hook that up like that . what we 're gon na do is we 're gon na generate this iv curve by making actual measurements of i and v. so my first v setting is zero , that gives me this point here , i hope i measure a current of zero , otherwise this thing would be generating power , which it 's not gon na do . and then i turn up the voltage slightly , and what i notice is there 's no current , there 's no current when it 's at point one volts , or point two volts . and then when it gets to around point six volts , on the diode , here 's vd , and here 's , when the voltage on the diode is around point six volts what i notice is the current goes up . so it goes up to five milliamps , and then a little bit higher , it goes up to ten milliamps , like that , and i can plot out all these points along this part of the curve . now , i go back here and i change the voltage here to read the other way around , and that means i 'm traveling this way on the voltage axis . and what i 'll read , my ammeter , will read zero milliamps . zero , zero , zero , zero , zero . and so they plot in this part of the line here . now if i make this voltage really large and really negative , say i make this like minus 50 volts , that 's this point here , what happens is i see a really sharp increasing current , like that right there , and it keeps going . and that is called the breakdown , vbr is breakdown . and for silicon diodes , minus 50 volts is a typical value for that . this graph here shows a break in the scale , so this is minus one volt , minus two volts , and then we go all the way out to 50 volts , minus 50 volts , and that 's where the breakdown occurs . and most of the time when we 're using diodes , we 're using them between plus or minus one volt across their terminals . that 's how we know what the iv characteristic of a diode is . and what we can do is actually , for this section of the curve right here , for this part of the curve , i can model this with an equation . and the equation looks like this . this is the iv equation for a diode , so this is sort of like the ohm 's law for a diode . i equals is , this is the current , times e to the q , that 's the charge on an electron , times v on the diode , that 's the voltage on the diode , divided by kt minus one . k is boltzmann 's constant , and t is the temperature of the device , measured in kelvin . so this equation actually fits this part of this curve for a real diode , it 's a fitting curve . we 'll look at these constants one at a time . is is called the saturation current . saturation current . and for silicon , for silicon that 's a value of about 10 to the minus 12 amperes , which is one picoampere , that 's how much is is . q is the charge on an electron , and that equals 1.602 times 10 to the minus 19 coulombs . that 's q , vd is the voltage across the diode , k is boltzmann 's constant , that 's a small k , usually , and that equals 1.38 times 10 to the minus 23 joules per kelvin . and the last variable is t , and that 's the temperature , and that 's measured in kelvin , with a big k. kelvin is the absolute temperature scale , so zero kelvin equals minus 273 degrees celsius . very , very cold . so this right here is the diode equation , that 's the diode iv equation . and it has this exponential shape in it , it has this exponential term in it , but when we look over here , maybe this does n't look like an exponential curve , you have n't seen a curve like that . but that actually is just a trick of the scale of this drawing , so what i wan na do now is i 'm gon na zoom in really super close , right on this origin right here , and we 're gon na see how this exponential term shows up , and we 'll see what the meaning of is is . i equals is times e qv over kt minus one , and here 's a close up , here 's an extreme close-up on the origin of the diode curve . the voltage scale is blown up by about a factor of 10 , so here 's 1/10th of a volt forward across the diode , and the current scale is super blown up , this is in picoamperes now , so this is in 10 to the minus 12th amperes instead of 10 to the minus three . and you can see here , this is a more familiar looking exponential curve . and over here there 's a little bit of an offset , there 's a little tiny current in the reverse direction when the voltage is negative . and this amount here , that 's is , flowing in the negative direction in the diode . if we look at the diode equation , and you let v go negative , what happens is this term here in the diode equation becomes very , very small compared to one . and what 's left is is times one , and that 's what we 're looking at right here . this is a really small current , as you can see from the scale here , it 's down in the low picoamps area . almost all the time you can ignore this current , and just treat it as zero . whenever i wan na use a diode in a circuit , and we 'll see how we solve circuits that include these non-linear diodes in them . |
| questionsrc | the source of the question | if it was a perfect diode , made in some unknown technology , what would happen is in the reverse direction , if the voltage across the diode was negative , we 'll label the voltage this way , if the voltage across the diode was negative , that is , this terminal is at a higher voltage than this terminal , there would be zero current flowing . and then for any positive voltage , basically the diode would look like a wire . so i can call that , that 's essentially model number zero of a diode .                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| question    | the text of the question   | what would a diode look like on a circuit board ?                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |