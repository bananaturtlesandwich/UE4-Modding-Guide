# Level Editing/Replacing
**The process is exactly the same as adding any level in unreal engine**

For now this just details replacing the course model but I do have a project brewing...
- First export the course model
- Open in your 3d software of choice and start editing/ replacing content
- If there also a model for damage zones then import that too
- All collision will have to be done manually
- In blender, to make collision you must name it UCX_*corresponding model*_*collision number*
- When adding collision use shapes with no inward sloping faces(cuboids and triangular prisms)
- Alternatively, you could turn on advanced collision in engine for convenience at the cost of extra processing needed for its calculation or add collision in the model viewer by turning on collision view
- Import the course model into the proper folders in your unreal project
- Link materials and material instances like normal
- Save content and package