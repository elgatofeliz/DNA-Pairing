# DNA-Pairing

FreeCodeCamp
    JavaScript Algorithms and Data Structures
    Intermediate Algorithm Scripting

DNA Pairing

Pairs of DNA strands consist of nucleobase pairs. Base pairs are represented by the characters AT and CG, which form building blocks of the DNA double helix.

The DNA strand is missing the pairing element. Write a function to match the missing base pairs for the provided DNA strand. For each character in the provided string, find the base pair character. Return the results as a 2d array.

For example, for the input GCG, return [["G", "C"], ["C","G"], ["G", "C"]]

The character and its pair are paired up in an array, and all the arrays are grouped into one encapsulating array.

--- Here's the Code ---

function pairElement(str) {
  return str.split("").map(elt => {
    if (elt === "A") return ["A", "T"]  
    if (elt === "C") return ["C", "G"]
    if (elt === "G") return ["G", "C"]
    if (elt === "T") return ["T", "A"]
  })
}

pairElement("GCG");
