itk_module_test()

#${itk-module} will be the name of this module and will not need to be
#changed when this module is renamed.

set(ITK${itk-module}Tests
  itkSeparableBinaryDilateImageFilterTest.cxx
  itkSeparableBinaryErodeImageFilterTest.cxx
)

CreateTestDriver(${itk-module}  "${ITK${itk-module}-Test_LIBRARIES}" "${ITK${itk-module}Tests}")
