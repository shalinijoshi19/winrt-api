---
-api-id: T:Windows.Data.Text.WordSegmentsTokenizingHandler
-api-type: winrt delegate
-api-device-family-note: xbox
---
<!-- Delegate syntax.
public delegate void WordSegmentsTokenizingHandler(Windows.Foundation.Collections.IIterable<Windows.Data.Text.WordSegment> precedingWords, Windows.Foundation.Collections.IIterable<Windows.Data.Text.WordSegment> words)
-->
# Windows.Data.Text.WordSegmentsTokenizingHandler

## -description
Defines the signature of a function that is provided to [WordsSegmenter.Tokenize](wordssegmenter_tokenize_982453003.md).

## -parameters
### -param precedingWords
Contains the selectable words, in reverse order, that precede the parameter *startIndex* that is provided to [WordsSegmenter.Tokenize](wordssegmenter_tokenize_982453003.md).

### -param words
Contains the selectable words that contain or follow the parameter *startIndex* that is provided to [WordsSegmenter.Tokenize](wordssegmenter_tokenize_982453003.md).


## -remarks
One iterator passed to the handler iterates through all the words in the provided text that occur prior to the parameter *startIndex* (passed to [Tokenize](wordssegmenter_tokenize_982453003.md)), in reverse order. The other iterator iterates through all the words in the provided text that contain or follow *startIndex*.

**Example**: If you provide [Tokenize](wordssegmenter_tokenize_982453003.md) with "this is a simple example" and *startIndex* within the word "simple", *precedingWords* iterates through the words "a ", "is ", "this ", and *words* iterates through the words "simple ", "example".

*precedingWords* and *words* are valid only during the lifetime of the handler.

## -examples

## -see-also
[WordsSegmenter.Tokenize](wordssegmenter_tokenize_982453003.md)