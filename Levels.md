# Level Editing/Replacing

*For Blue Fire, the process in easier for voids as all other environments do not use dynamic lighting*
*The process is basically the same as adding any level in unreal engine*

- First export the level model using umodel
- Open in your 3d software of choice and start editing/ replacing content
- If there also a model for damage zones then import that too
- All collision will have to be done manually(In blender, to make collision you must put UCX_*model*_*collision number*(if you put collision all in one model then it will be merged in engine))
- When adding collision use shapes with no inward sloping faces(cuboids and triangular prisms)
- Alternatively, you could turn on advanced collision in engine for convenience at the cost of extra processing needed for its calculation or add collision in the model viewer by turning on collision view
- Set up a UE4 project(turn off use pak file) and import the course model into the proper folders
- Link materials and material instances like normal
- save content and package
