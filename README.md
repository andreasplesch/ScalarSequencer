# ScalarSequencer
ScalarSequencer is a X3D event utility node and is also known as FloatSequencer. Its functionality parallels the BooleanSequencer and IntegerSequencer nodes but provides value_changed field values of type SFFloat instead.

# Motivation
ScalarSequencer is similar to ScalarInterpolator but provides extra `next` and `previous` fields, and a stepwise evaluation. It allows for stepping through float values for discrete control of many properties such as transparency or shininess. Routed through interpolators it allows also sequencing colors, positions, orientations or coordinates.

# Signature
```
ScalarSequencer : X3DSequencerNode {
  SFBool  [in]     next
  SFBool  [in]     previous
  SFFloat [in]     set_fraction
  MFFloat [in,out] key           []   (-∞,∞) 
  MFFloat [in,out] keyValue      []   (-∞,∞)
  SFNode  [in,out] metadata      NULL [X3DMetadataObject]
  SFFloat [out]    value_changed
}
```
# Prototype
