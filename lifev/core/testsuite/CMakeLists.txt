
INCLUDE(TribitsAddExecutableAndTest)
INCLUDE(AddSubdirectories)

ADD_SUBDIRECTORIES(
  adr_assembler
  array
  bdf
  fe_function
  fem
  filter
  hyperbolic
  linear_solver
  linear_solver_preconditioner
  matrix_epetra_structured_framework
  mesh
  region_marker_id
  partition_io
  template_test
  vector_container
)

IF(LifeV_${PACKAGE_NAME}_ENABLE_SPIRIT_PARSER)
  ADD_SUBDIRECTORY(parser)
ENDIF()
