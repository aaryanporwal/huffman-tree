# Huffman Tree Project

# ABSTRACT

Data compression is also called source coding. It is the process of encoding information using fewer bits than a raw representation, making use of specific encoding schemes. Compression is a technology for reducing the quantity of data used to represent any content without excessively reducing the quality of the data. It also reduces the number of bits required to store and/or transmit digital media. There are various techniques available for compression, In this project we have used the Huffman algorithm for text compression.


Huffman Coding is a lossless compression algorithm which, given a sequence of characters, generates a set of binary encoding for each character in the sequence. The generated binary codes are said to be Optimal Prefix Codes; this implies two things:

* The binary encoding for one character cannot be the prefix of that for another character. This prevents us from having to include a separator between the Huffman codes for two characters to avoid ambiguity while decoding the encoded sequence.
* The generated codes are optimal in the sense that the length of the binary code is directly proportional to the frequency of its occurrence in the given sequence. This means that the most frequently used symbol will have the shortest length code, while the least frequently used symbol will have the longest. 

This is great for static files like HTML, CSS and JavaScript files which have a lot of repetitive tokens.


# DESIGN OF THE PROJECT -
This project makes use of concepts of File Handling in C++, Binary Heaps and Huffman Coding Algorithms.

The program first reads a file, consisting of any type of HTML, CSS, JSON etc. files. 

The file elements are read character-wise and a binary heap is created on the basis of frequency of characters encountered in the file. 

This binary heap(that maintains an optimal merge pattern) is then used to create a Huffman tree.

The formation of the Huffman Tree has been represented in the Output section of the implementation. 

These Huffman trees can then be used to encode and/or decode any type of code or text, respectively.


![Output](https://lh3.googleusercontent.com/iMIwbKNVbw_mQEmRNqazZJwiak3hcnByybF37G-Zp2yqLqgHmiZUF7sw2Webawqe4uQySjvfTsxST6fcGk_BFg-qthaaoAFUB9Yj4RZpzFVH5wmSnSDJP_Dubzz27Qi-a4KhAYbW)
![](https://lh6.googleusercontent.com/EyFSXzTKSWSvv_iCQ9392pPqf5iuwMLP--O3F0IH8l9PkYYofJqwsM1DwfE7vEpZETrsIbQ7KczQiTIq9J1BGBt0SERPV7yLyBjDh0S0UtgAkikgFgWWozmKJLC_eLJ7dycxXdjq)
![](https://lh5.googleusercontent.com/IBMWEeUuT0RpM9lBmBArgfFpj-aw4U9aJIMCEGSpfS7zpYb7HQcZYAG0LLgmDeiuyWAOYm6Kd6_Sh4JDlKwaKQ5Ou04nG-hHInjBLizyQJiWcJFE7aNFx_poCjsWY1SwUdkERkEW)
![](https://lh4.googleusercontent.com/9Vu6dPCsE36KOnIyMbYw9V-TJY_Ag2Xc4ng7sHomoJDdEhLvZdwiOde6N2d8YX_sEzeGtc-pjjM04K5c7aF0l3Ynn9CfLWre9QnxI-bBCr5qd2dDu9DzlU_xW5h8CTBsPk2ZCI7_)
