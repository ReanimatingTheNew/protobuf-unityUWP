This directory contains the C# Protocol Buffers runtime library.
It is slightly modified to work with unity and unity UWP builds at .Net 4.6

Usage
=====

Import the plugin to unity

History of C# protobufs
=======================

This subtree was originally imported from https://github.com/jskeet/protobuf-csharp-port
and represents the latest development version of C# protobufs, that will now be developed
and maintained by Google. All the development will be done in open, under this repository
(https://github.com/google/protobuf).

The previous project differs from this project in a number of ways:

- The old code only supported proto2; the new code only supports
proto3 (so no unknown fields, no required/optional distinction, no
extensions)
- The old code was based on immutable message types and builders for
them
- The old code did not support maps or `oneof`
- The old code had its own JSON representation, whereas the new code
uses the standard protobuf JSON representation
- The old code had no notion of the "well-known types" which have
special support in the new code
- The old project supported some older platforms (such as older
versions of Silverlight) which are not currently supported in the
new project
