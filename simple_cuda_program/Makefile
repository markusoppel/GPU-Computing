CXX := nvcc
TARGET := vector_add
SRC := vector_add.cu

.PHONY: all clean

all: $(TARGET)

$(TARGET): $(SRC)
	$(CXX) -o $@ $^

run: $(TARGET)
	./$(TARGET)

clean:
	rm -f $(TARGET)