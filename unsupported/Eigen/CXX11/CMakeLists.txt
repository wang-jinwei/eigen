set(Eigen_CXX11_HEADERS Tensor TensorSymmetry ThreadPool)

if(TOP_PROJECT)
  install(FILES
    ${Eigen_CXX11_HEADERS}
    DESTINATION ${INCLUDE_INSTALL_DIR}/unsupported/Eigen/CXX11 COMPONENT Devel
    )
  install(DIRECTORY src DESTINATION ${INCLUDE_INSTALL_DIR}/unsupported/Eigen/CXX11 COMPONENT Devel FILES_MATCHING PATTERN "*.h")
endif()
