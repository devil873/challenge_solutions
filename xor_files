import sys

count = 0
for file1 in range(1,21):
	file1_b = bytearray(open(str(file1)+".key", 'rb').read())
	for file2 in range(file1+1,21):
		file2_b = bytearray(open(str(file2)+".key", 'rb').read())

		# Set the length to be the smaller one
		size = len(file1_b) if len(file1_b) < len(file2_b) else len(file2_b)
		xord_byte_array = bytearray(size)

		# XOR between the files
		for i in range(size):
			xord_byte_array[i] = file1_b[i] ^ file2_b[i]
		count +=1
		try:
			x=xord_byte_array.decode()
		except:
			x=0
		print("Number: "+str(count)+"\n"+str(x)+"\n\n")
