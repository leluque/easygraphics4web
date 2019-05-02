This document presents a quick tour to the EasyGraphics4Web library.

# Purpose

EasyGraphics4Web is a client-side Typescript library designed to make it easier and more flexible the manipulation of geometric shapes, text, and connection paths. The main reason for its creation was the preparation of a structure that could be used in libraries for the representation and manipulation of diagrams.

# Main Design And Usage Requirements

EasyGraphics4Web has been developed having in mind some design requirements and usage purposes:
* It must provide a layer that is independent of the drawing library (e.g. SVG.js, Snap.svg, Paper.js) and technology (e.g. SVG, canvas) used;
* It must support drawing, manipulating, and animating shapes/text, as well as attaching events to them;
* It must implement different layouts, allowing automatic organization of shapes/text (e.g. horizontal and vertical linear layouts);
* It must support different look-and-feels