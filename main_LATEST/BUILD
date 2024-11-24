load(
      "@rules_cc//cc:defs.bzl"
   ,  "cc_library"
   ,  "cc_binary"
)

cc_library(
      name = "common"
   ,  hdrs = [
            "source/common/TypesStd.hpp"
      ]
   ,  includes   = ["./source/common"]
   ,  visibility = ["//visibility:public"]
)

cc_library(
      name = "aapFunctionalCluster_DiagnosticManagement"
   ,  srcs = ["source/aapFunctionalCluster_DiagnosticManagement/aapFunctionalCluster_DiagnosticManagement.cpp"]
   ,  deps = [
            "//repo_projects/pProjectDiagnosticTester/main_LATEST:common"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:SwcServiceEcuM"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:SwcServiceEthTp"
      ]
   ,  hdrs = [
            "source/aapFunctionalCluster_DiagnosticManagement/infClientSwcServiceDcm.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_CancellationHandler.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_Condition.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_Conversation.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_DTCInformation.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_Event.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_Indicator.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_MetaInfo.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_Monitor.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_MultipleCondition.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_MultipleEvent.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_MultipleMonitor.hpp"
         ,  "source/aapFunctionalCluster_DiagnosticManagement/interface_DiagnosticManagement_OperationCycle.hpp"
      ]
   ,  includes   = ["./source/aapFunctionalCluster_DiagnosticManagement"]
   ,  visibility = ["//visibility:public"]
)

cc_library(
      name = "aapFunctionalCluster_ExecutionManagement"
   ,  srcs = ["source/aapFunctionalCluster_ExecutionManagement/aapFunctionalCluster_ExecutionManagement.cpp"]
   ,  deps = [
            "//repo_projects/pProjectDiagnosticTester/main_LATEST:common"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:aapFunctionalCluster_DiagnosticManagement"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:SwcServiceEcuM"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:SwcServiceEthTp"
      ]
   ,  hdrs = [
            "source/aapFunctionalCluster_ExecutionManagement/interface_ExecutionManagement_ExecutionClient.hpp"
      ]
   ,  includes   = ["./source/aapFunctionalCluster_ExecutionManagement"]
   ,  visibility = ["//visibility:public"]
)

cc_library(
      name = "SwcServiceEcuM"
   ,  srcs = ["source/SwcServiceEcuM/SwcServiceEcuM.cpp"]
   ,  deps = [
            "//repo_projects/pProjectDiagnosticTester/main_LATEST:common"
      ]
   ,  hdrs = [
            "source/SwcServiceEcuM/infClientSwcServiceEcuM.hpp"
      ]
   ,  includes   = ["./source/SwcServiceEcuM"]
   ,  visibility = ["//visibility:public"]
)

cc_library(
      name = "SwcServiceEthTp"
   ,  srcs = [
            "source/SwcServiceEthTp/SwcServiceEthTp.cpp"
      ]
   ,  deps = [
            "//repo_projects/pProjectDiagnosticTester/main_LATEST:common"
         ,  "//repo_projects/pProjectVirtualEcu/main_LATEST:aapFunctionalCluster_Persistency"
      ]
   ,  hdrs = [
            "source/SwcServiceEthTp/infClientSwcServiceEthTp.hpp"
      ]
   ,  includes   = ["./source/SwcServiceEthTp"]
   ,  visibility = ["//visibility:public"]
)

cc_binary(
      name = "pProjectDiagnosticTester_main_LATEST"
   ,  deps = [
            "//repo_projects/pProjectDiagnosticTester/main_LATEST:common"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:aapFunctionalCluster_DiagnosticManagement"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:aapFunctionalCluster_ExecutionManagement"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:SwcServiceEcuM"
         ,  "//repo_projects/pProjectDiagnosticTester/main_LATEST:SwcServiceEthTp"
      ]
   ,  visibility = ["//visibility:public"]
)

