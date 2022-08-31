all: TextTrader_TTS TextTrader_simnow
TextTrader_TTS:
	g++ -std=c++11 -I. -I../../CTP -I../../INIReader -L/lib64 -L../.. -finput-charset=UTF-8 -fexec-charset=UTF-8 -o $@ ../../TextTrader.cpp ../../INIReader/INIReader.cpp ../../INIReader/ini.c thostmduserapi_se_tts.so thosttraderapi_se_tts.so -lncursesw -ltinfo

TextTrader_simnow:
	g++ -std=c++11 -I. -I../../CTP -I../../INIReader -L/lib64 -L../.. -finput-charset=UTF-8 -fexec-charset=UTF-8 -o $@ ../../TextTrader.cpp ../../INIReader/INIReader.cpp ../../INIReader/ini.c thostmduserapi_se_v667.so thosttraderapi_se_v667.so -lncursesw -ltinfo

clean:
	rm -f TextTrader_TTS TextTrader_simnow

