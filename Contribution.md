# Cnntribution guide line
 This repository contains Android code, means java code, so you should follow some rules to write code. Here they are

### 1. Follow Field Naming Conventions

>Non-public, non-static field names start with m.

>Static field names start with s.

>Other fields start with a lower case letter.

>Public static final fields (constants) are ALL_CAPS_WITH_UNDERSCORES.

For example:

        public class MyClass {
            public static final int SOME_CONSTANT = 42;
            public int publicField;
            private static MyClass sSingleton;
            int mPackagePrivate;
            private int mPrivate;
            protected int mProtected;
        }

### 2. Use Standard Brace Style

Braces do not go on their own line; they go on the same line as the code before them:

        class MyClass {
            int func() {
                if (something) {
                   // ...
                } else if (somethingElse) {
                    // ...
                } else {
                   // ...
                }
            }
        }

We require braces around the statements for a conditional. Exception: If the entire conditional (the condition and the body) fit on one line, you may (but are not obligated to) put it all on one line. For example, this is acceptable:

        if (condition) {
            body();
        }

and this is acceptable:

        if (condition) body();

but this is not acceptable:

        if (condition)
            body();  // bad!


### 3. Treat Acronyms as Words

Treat acronyms and abbreviations as words in naming variables, methods, and classes to make names more readable:

 Good |	          Bad |
 ------------ | -----------: |
 XmlHttpRequest |           	 XMLHTTPRequest |
 getCustomerId |	             getCustomerID |     
 class Html |	                 class HTML |
 String url |	                 String URL |
 long id |	                     long ID |

As both the JDK and the Android code bases are very inconsistent around acronyms, it is virtually impossible to be consistent with the surrounding code. Therefore, always treat acronyms as words.


### 4. Use TODO Comments

Use TODO comments for code that is temporary, a short-term solution, or good-enough but not perfect. TODOs should include the string TODO in all caps, followed by a colon:

    // TODO: Remove this code after the UrlTable2 has been checked in.

and

    // TODO: Change this to use a flag instead of a constant.

If your TODO is of the form "At a future date do something" make sure that you either include a very specific date ("Fix by November 2005") or a very specific event ("Remove this code after all production mixers understand protocol V7.").

### 5. Log

Usually, we use Toast to test some fucntion and more. You should use log instead of toast to save your time with getting a good feel of programming with big toast text.

Apart from these rules you can find more here with java reference [link](https://source.android.com/setup/code-style)


We are welcoming to contributors, so you are eagily waiting for get a PR accepted and issue get resolved.
