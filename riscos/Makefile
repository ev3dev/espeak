# Project:   Speak3


# Toolflags:
CCflags = -c -C90 -depend !Depend -IC: -throwback -zM
C++flags = -c -depend !Depend -IC: -throwback -zM
Linkflags = -rmf -c++ -o $@
ObjAsmflags = -throwback -NoCache -depend !Depend
CMHGflags = 
LibFileflags = -c -o $@
Squeezeflags = -o $@


# Final targets:
@.speakmod:   @.o.speak_riscos @.o.compiledict @.o.dictionary \
        @.o.intonation @.o.readclause @.o.setlengths @.o.synthdata \
        @.o.synthesize @.o.translate  @.o.tr_languages \
        @.o.tr_english @.o.wavegen @.o.voices @.o.assemb @.o.cmhgfile
        Link $(Linkflags) C:o.stubs C:o.c++lib @.o.speak_riscos @.o.compiledict \
        @.o.dictionary @.o.intonation @.o.readclause @.o.setlengths \
        @.o.synthdata @.o.synthesize \
        @.o.translate @.o.tr_english @.o.wavegen @.o.tr_languages \
        @.o.voices @.o.assemb @.o.cmhgfile


# User-editable dependencies:

# Static dependencies:
@.o.speak_riscos:   @.cpp.speak_riscos
        c++ $(c++flags) -o @.o.speak_riscos @.cpp.speak_riscos 
@.o.compiledict:   @.cpp.compiledict
        c++ $(c++flags) -o @.o.compiledict @.cpp.compiledict 
@.o.dictionary:   @.CPP.dictionary
        c++ $(c++flags) -o @.o.dictionary @.CPP.dictionary 
@.o.intonation:   @.CPP.intonation
        c++ $(c++flags) -o @.o.intonation @.CPP.intonation
@.o.readclause:   @.CPP.readclause
        c++ $(c++flags) -o @.o.readclause @.CPP.readclause
@.o.setlengths:   @.CPP.setlengths
        c++ $(c++flags) -o @.o.setlengths @.CPP.setlengths 
@.o.synthdata:   @.CPP.synthdata
        c++ $(c++flags) -o @.o.synthdata @.CPP.synthdata 
@.o.synthesize:   @.CPP.synthesize
        c++ $(c++flags) -o @.o.synthesize @.CPP.synthesize 
@.o.translate:   @.CPP.translate
        c++ $(c++flags) -o @.o.translate @.CPP.translate 
@.o.tr_english:   @.CPP.tr_english
        c++ $(c++flags) -o @.o.tr_english @.CPP.tr_english 
@.o.tr_languages:   @.CPP.tr_languages
        c++ $(c++flags) -o @.o.tr_languages @.CPP.tr_languages 
@.o.voices:   @.CPP.voices
        c++ $(c++flags) -o @.o.voices @.CPP.voices 
@.o.wavegen:   @.CPP.wavegen
        c++ $(c++flags) -o @.o.wavegen @.CPP.wavegen 
@.o.assemb:   @.s.assemb
        objasm $(objasmflags) -from @.s.assemb -to @.o.assemb

# Dynamic dependencies:
