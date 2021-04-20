# Questions

## What's `stdint.h`?

stdint.h is a header file in the C standard library introduced in the C99 standard library section 7.18 to allow programmers to write more portable code by providing a set of typedefs that specify exact-width integer types

## What's the point of using `uint8_t`, `uint32_t`, `int32_t`, and `uint16_t` in a program?

These functions are a cross-platform implementation of a standard data type.

## How many bytes is a `BYTE`, a `DWORD`, a `LONG`, and a `WORD`, respectively?

1, 4, 4, 2

## What (in ASCII, decimal, or hexadecimal) must the first two bytes of any BMP file be? Leading bytes used to identify file formats (with high probability) are generally called "magic numbers."

Hex:    0x424d

## What's the difference between `bfSize` and `biSize`?

bfSize is the size of the bmp file. biSize is the size of the structure. Both in bytes.

## What does it mean if `biHeight` is negative?

If biHeight is negative, indicating a top-down DIB, biCompression must be either BI_RGB or BI_BITFIELDS.

## What field in `BITMAPINFOHEADER` specifies the BMP's color depth (i.e., bits per pixel)?

biBitCount specifies the BMP's color depth - the number of bits per pixel.

## Why might `fopen` return `NULL` in `copy.c`?

fopen might return a NULL pointer if the file that fopen is trying to write to doesn't exist

## Why is the third argument to `fread` always `1` in our code?

fread's third argument is always 1 cause we are iterating over every pixel.

## What value does `copy.c` assign to `padding` if `bi.biWidth` is `3`?

This step ensures the number of bytes in every row is a multiple of 4.

## What does `fseek` do?

fseek allows us to change the offset of a pointer.

## What is `SEEK_CUR`?

SEEK_CUR is the current position indicator in the file.
