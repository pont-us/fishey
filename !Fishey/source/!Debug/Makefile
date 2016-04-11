# This makefile made by Makatic2



ObjectFiles	=		\
			o.appshell	\
			o.choices	\
			o.main	\


ProjectName		=	!Debug

Libraries = OSLib:o.OSLib C:o.stubs C:o.flexlib

Target = ^.^.!Fishey.!RunImage

ASMFlags  = $(ASMExtra) -Stamp -NoCache -CloseExec -Quit -throwback
CCFlags   = $(CCExtra) -D__swi -fussy -fah -depend !Depend -throwback -I,@.^,C:,OS:
CPPFlags  = $(CPPExtra) -depend !Depend -throwback -I,@.^,C:
LinkFlags = $(LinkExtra)

ASM  = objasm $(ASMFlags)
CC   = cc -c $(CCFlags)
CPP  = Makatic._C++ c++ -c $(CPPFlags)
LINK = Link -aif -c++ $(LinkFlags)



# Don't alter anything below this...


VPATH = @.^

.SUFFIXES: .o .s .c .c++

$(Target): $(ObjectFiles) $(ExtraLibs) $(Libraries)
           $(LINK) -o $@ $(ObjectFiles) $(ExtraLibs) $(Libraries)
           Settype $@ ff8

.s.o:
           $(ASM) -from $< -to $@

.c.o:
           $(CC) -o $@ $<

.c++.o:
           $(CPP) -o $@ $<


# Dynamic dependencies:
o.appshell:	^.c.appshell
o.appshell:	C:h.application
o.appshell:	C:h.bool
o.appshell:	C:h.types
o.appshell:	C:h.toolbox
o.appshell:	C:h.os
o.appshell:	C:h.wimp
o.appshell:	C:h.osspriteop
o.appshell:	C:h.font
o.appshell:	C:h.messagetrans
o.appshell:	C:h.error
o.appshell:	C:h.exception
o.appshell:	C:h.nevent
o.appshell:	C:h.nev_toolbox
o.appshell:	C:h.nevent
o.appshell:	C:h.nev_message
o.appshell:	C:h.nevent
o.appshell:	^.h.choices
o.choices:	^.c.choices
o.choices:	C:h.optionbutton
o.choices:	C:h.types
o.choices:	C:h.toolbox
o.choices:	C:h.os
o.choices:	C:h.wimp
o.choices:	C:h.osspriteop
o.choices:	C:h.font
o.choices:	C:h.messagetrans
o.choices:	C:h.gadget
o.choices:	C:h.numberrange
o.choices:	C:h.nev_toolbox
o.choices:	C:h.nevent
o.choices:	^.h.main
o.choices:	^.h.choices
o.main:	^.c.main
o.main:	C:h.os
o.main:	C:h.types
o.main:	C:h.hourglass
o.main:	C:h.shifting
o.main:	C:h.messagetrans
o.main:	C:h.allocate
o.main:	^.h.appshell
o.main:	C:h.bool
o.main:	C:h.exception
o.main:	C:h.nev_wimp
o.main:	C:h.nevent
o.main:	C:h.toolbox
o.main:	C:h.wimp
o.main:	C:h.osspriteop
o.main:	C:h.font
o.main:	C:h.nev_message
o.main:	C:h.nevent
o.main:	C:h.nev_toolbox
o.main:	C:h.nevent
o.main:	C:h.window
o.main:	C:h.keyboardshortcut
o.main:	C:h.gadget
o.main:	^.h.choices
o.main:	^.h.main
