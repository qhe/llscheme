SOURCE := $(wildcard *.cc)
OBJECT := $(SOURCE:.cc=.o)

CXXFLAGS += -W -Wall -I./include

TARGET := mylexer

all: $(TARGET)

.PHONY: clean
clean:
	$(RM) $(TARGET) $(OBJECT)

$(TARGET): $(OBJECT)
	$(CXX) $(CXXFLAGS) $^ -o $@
