INCLUDES = -I"../../allegro-5.2.3.0/include/" -I"../../allegro-5.2.3.0/build/include/" -I"../../allegro-5.2.3.0/addons/image/"
LIBDIRS = -L"../../allegro-5.2.3.0/build/lib/"
LIBS = -lallegro -lallegro_image
TARGET = decompress

all: $(TARGET)

decompress.o: decompress.cpp
	g++ -c $(INCLUDES) $(LIBS)  decompress.cpp 


$(TARGET): decompress.o
	 g++ decompress.o $(LIBDIRS) $(LIBS) -o $(TARGET)
	 
clean:
	-rm $(TARGET) decompress.o
	
