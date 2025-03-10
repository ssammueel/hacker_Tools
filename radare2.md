# radare2
- this is a s a reverse-engineering tool.
- reverse engineering involves involves analyzing software or hardware to understand its design,how it operates

  to open radare2 we use
  
![Image](https://github.com/user-attachments/assets/363cea7b-ae42-4191-a6ac-847f80e33f04)

### controls
##### 1. ?
- this is like help, it shows commands we have in radere2

![Image](https://github.com/user-attachments/assets/2e5f5ab5-5c9b-4741-b352-78a63c86031c)

#### 2. aaa
- this shows you what steps radare2 takes. Each step has the command responsible for it inside parentheses. It looks for executable sections and looks for calls. when it finds a call, it looks for the destination of the call. Splits up basic blocks, and tries to remove all the false positives.

![Image](https://github.com/user-attachments/assets/c3843d71-c326-4e18-81f0-989be7072ec9)

#### 3.afl

- afl stands for Analyze Functions List.Running afl after analysis provides details such as function addresses, sizes, types, and names.

![Image](https://github.com/user-attachments/assets/bb0e7f49-0ef5-4c9b-abe2-a69f8a4e7234)
  
#### 4. V
- it will show us all the different types of views we have in the tool.
- to navigate between the views we press the letter ‘p’.

![Image](https://github.com/user-attachments/assets/545b112c-722b-4574-85e6-97c876c72208)

#### 5. i
is used for information gathering about the loaded binary.

Common i Commands:
> i → Show general binary info (architecture, format, size, etc.).]  
> ii → List imported symbols (functions from shared libraries).  
> il → List linked libraries.  
> is → Show symbols (functions, variables, etc.).  
> iz → List strings found in the binary.iS → Show binary sections.  
> iM → Display memory maps (useful when debugging).  

#### 2.#### 2.#### 2.#### 2.#### 2.#### 2.#### 2.
