# Hello-World
My name is Luhan Monat.  I have spent most of my working carrier in electronics working with microprocessors and microcontrollers.

I've done a shitload of PIC programming.  I really like the total control of assembly language coding.

Then I discovered Arduino ...

Arduino uses a very good C compiler that does much more than Arduino lets on.  In addition to the C++ extensions, you get full (kinda) K&R C.  This includes: structures, unions, typedefs, enums, and multidimensional arrays.

A few of the fucntions like 'printf' are missing but you can simulate them using 'sprintf'.

When you select a 'board' - i.e. chip, you get full named access to every single one of it's registers.  This virtually eliminates the need to resort to inline assembler for tricky operations.

The big advantage of the Arduino development environment is the use of bootloaders in any of the IC's that it can use.  This makes it 'one click' to download and run your program right from the source file editor.

The 'Setup' and 'Loop' structure is a bit hokey but it is used to load the support code for their C++ extensions (delay,Serial.print, etc).  However...

You can replace them with a standard 'int main()' and write all of your code that way.  This appoximates the 'total control' I used to have writing assembler on PIC chips.  You lose some of the C++ extensions like delay, but you still get delayMicroseconds to with a couple lines of code you can implement that function yourself.

I have a bunch of Atmel micros that I have preloaded with bootloaders.  These become 'Arduinos' by using a cheapo USB to TTL converter.  One click and way you go.
