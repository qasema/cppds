..  Copyright (C)  Brad Miller, David Ranum, and Jan Pearce
    This work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/.


Reviewing Basic C++
-------------------

In this section, we will review the programming language C++ and also
provide some more detailed examples of the ideas from the previous
section. If you are new to C++ or find that you need more information
about any of the topics presented, we recommend that you consult a resource such as
the `C++ Reference <http://www.cplusplus.com/reference/>`_
or a `C++ Tutorial <http://www.cplusplus.com/doc/tutorial/>`_.
Our goal
here is to reacquaint you with the C++ language and also reinforce some of
the concepts that will be central to later chapters.

C++ is an object-oriented programming language.
It has a powerful set of built-in data types and control
constructs. Since C++ is a compiled language, all the code written in this language,
when run, are translated to **machine code** by a program called the **compiler**.

The following is an example of C++ code that writes to the console:

.. activecode:: cpp
  :caption: A simple C++ program with output
  :language: cpp

  //Outputs strings to command line.
  #include <iostream>
  using namespace std;

  int main() {
      cout << "Welcome to Problem Solving with" << endl;
      cout << "Algorithms and Data Structures!" << endl;
      return  0;
  }

  

.. activecode:: cpp_units_1
    :language: cpp
    :autograde: unittest

    Write a function to compute the sum of num1 and num2
    ~~~~

    #include <iostream>
    using namespace std;

    int Sum(int num1, int num2 ) {
        //return 
    }


    ====

    #define CATCH_CONFIG_MAIN // This tells Catch to provide a main() - only do   this in one cpp file
    #include <catch.hpp>

    TEST_CASE("Failed test cases") {
    REQUIRE( Sum(1,4) == 5 );
    REQUIRE( Sum(2,4) == 6 );
    REQUIRE( Sum(0,0) == 0 );
    REQUIRE( Sum(5,0) == 5 );
    REQUIRE( Sum(-5,3) == -2 );
    REQUIRE( Sum(100,120) == 220 );
    
    }



.. activecode:: cpp_units_2
    :language: cpp
    :autograde: unittest

    Write a function that removes all the vowels from myword
    ~~~~

    #include <iostream>
    using namespace std;

    string vowels(string myword){


    }


    ====

    #define CATCH_CONFIG_MAIN // This tells Catch to provide a main() - only do   this in one cpp file
    #include <catch.hpp>

    TEST_CASE("Failed test cases") {
    REQUIRE( vowels("hello") == "hll" );
    REQUIRE( vowels("eau") == "" );
    REQUIRE( vowels("myth") == "myth" );
    REQUIRE( vowels("Welcome") == "Wlcm" );
    REQUIRE( vowels("books") == "bks" );
    REQUIRE( vowels("Fall2021") == "fll2021" );


    }


    