# PIT Primitive Spec-v1.2

## Version Update Instruction

| Date       | Version | Introduction                                  |
| ---------- | ------- | --------------------------------------------- |
| 2021.01.29 | v1.0    | First created                                 |
| 2021.03.02 | v1.1    | Some functions are deleted, added and changed |
| 2021.03.16 | v1.2    | Save functions added and other changes        |

* Modification in v1.1:

  > * Delete the `bmask` option in load functions. #Finished
  > * Add two new function: `split`and `merge`, which can spit and merge the elements of the ***Vector*** in bytes. #Finished
  > * Add a new option: `expand`, which indicates whether the data-width of the elements in the returned ***Vector*** is longer than that of the elements in the original one. #Finished
  > * Add a new option: `source<size>` , which can be used in the function `mskselect`. #Finished
  > * Change the input of some functions from pointer to data itself. #Finished
  > * Replace the function `actcsort` with two new functions: `acsort` and `tcsort`. #Finished
  > * Add a new data type: ***Ctrlword***, which can be used as the control word of the transmission process. #Finished
  > * Add a new option: `block<size_x>x<size_y>x<size_z>`, which can show the data structure information. #Finished
  > * Add a new option: `axis<xyz>`, which can show the order of the axes after transpose. #Finished
  > * Change `transpose` to support the transpose of 2d-array and 3d-array. #Finished
  > * Add a new function: `reorder`, which can support data reordering with ***Ctrlword***. #Finished
  > * Add two options: `max` and `min`, which can be used in the sorting functions. #Finished
  > * Change the function `sum` to support the `bmask` option. #Finished

* Modification in v1.2:

  > * Add a new option: `bbmask` , which can get the available situation of the each bit of every element. #Finished
  > * Change `mskselect` to support `bbmask`. #Finished
  > * Add two new options: `compress` and `decompress`. Compress the data when save it to memory and decompress the data when load it from the memory. #Finished
  > * Add a new function: `save`, save data to memory. #Finished
  > * Delete the ***Constant*** data type. #Finished
  > * Add a new option: `inbit` for `uniload` and `unisave`, which can help loading or saving data as the elements in bit. #Finished
  > * The output data format of `mskselect` is specified. #Finished
  > * Add a new Instance for Sparse DNN. #Achieve Phased Goals
