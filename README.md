# clion-cpp51382
Test repo for Clion issue CPP-51382

1. Sync the repo

2. Build it, ```bazel build //...```

3. Create a bazel run configuration to run the test suite as a whole, i.e 'bazel test //...'

4. Select and run the created test configuration from the Configuration pulldown

5. Observe that the test 'Adder - Simple/1 + 2' is yellow in the left hand pane of the Run/Tets window

6. Click on it, the info window changes to 

```
theAdder.add(1, 2) == 5
FAILED:
  CHECK(  )
with expansion:
  3 == 5
at test/adder/adder_tests.cpp:16
```
The source line is not underlined as a link, even if it was I would expect to go straight to the test 
fail line in the editor when clicked.

Note also that right clicking the entry shows a highlight with 'Nothing here' in it.