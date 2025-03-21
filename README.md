# RevolutionEHR_Downloader

## WSDL url
`https://services.revolutionehr.com/ws/services/partner?wsdl`

## Install `zeep` package
`pip install zeep`

## Get WSDL with `zeep`
`python -mzeep https://services.revolutionehr.com/ws/services/partner?wsdl`
```
Prefixes:
     xsd: http://www.w3.org/2001/XMLSchema
     ns0: http://ws.partner.revolutionehr.com

Global elements:
     ns0:WebServiceException(ns0:WebServiceException)
     ns0:activatePatient(ns0:activatePatient)
     ns0:activatePatientResponse(ns0:activatePatientResponse)    
     ns0:addPatient(ns0:addPatient)
     ns0:addPatientResponse(ns0:addPatientResponse)
     ns0:cancelAppointment(ns0:cancelAppointment)
     ns0:cancelAppointmentResponse(ns0:cancelAppointmentResponse)
     ns0:confirmAppointment(ns0:confirmAppointment)
     ns0:confirmAppointmentResponse(ns0:confirmAppointmentResponse)
     ns0:createAppointmentFromDetails(ns0:createAppointmentFromDetails)
     ns0:createAppointmentFromDetailsResponse(ns0:createAppointmentFromDetailsResponse)
     ns0:createAppointmentFromSlot(ns0:createAppointmentFromSlot)
     ns0:createAppointmentFromSlotResponse(ns0:createAppointmentFromSlotResponse)
     ns0:deactivatePatient(ns0:deactivatePatient)
     ns0:deactivatePatientResponse(ns0:deactivatePatientResponse)
     ns0:deceasePatient(ns0:deceasePatient)
     ns0:deceasePatientResponse(ns0:deceasePatientResponse)
     ns0:echo(ns0:echo)
     ns0:echoResponse(ns0:echoResponse)
     ns0:getAccountSummaryWithInsurance(ns0:getAccountSummaryWithInsurance)
     ns0:getAccountSummaryWithInsuranceResponse(ns0:getAccountSummaryWithInsuranceResponse)
     ns0:getAllEmployees(ns0:getAllEmployees)
     ns0:getAllEmployeesResponse(ns0:getAllEmployeesResponse)
     ns0:getAllProviders(ns0:getAllProviders)
     ns0:getAllProvidersResponse(ns0:getAllProvidersResponse)
     ns0:getAppointmentById(ns0:getAppointmentById)
     ns0:getAppointmentByIdResponse(ns0:getAppointmentByIdResponse)
     ns0:getAppointmentDetailById(ns0:getAppointmentDetailById)
     ns0:getAppointmentDetailByIdResponse(ns0:getAppointmentDetailByIdResponse)
     ns0:getApptTypes(ns0:getApptTypes)
     ns0:getApptTypesResponse(ns0:getApptTypesResponse)
     ns0:getEmployeeIdByProviderId(ns0:getEmployeeIdByProviderId)
     ns0:getEmployeeIdByProviderIdResponse(ns0:getEmployeeIdByProviderIdResponse)
     ns0:getEmployeeOffices(ns0:getEmployeeOffices)
     ns0:getEmployeeOfficesResponse(ns0:getEmployeeOfficesResponse)
     ns0:getEmployees(ns0:getEmployees)
     ns0:getEmployeesResponse(ns0:getEmployeesResponse)
     ns0:getEncounterById(ns0:getEncounterById)
     ns0:getEncounterByIdResponse(ns0:getEncounterByIdResponse)
     ns0:getInsuranceCompanies(ns0:getInsuranceCompanies)
     ns0:getInsuranceCompaniesResponse(ns0:getInsuranceCompaniesResponse)
     ns0:getInvoiceNotes(ns0:getInvoiceNotes)
     ns0:getInvoiceNotesResponse(ns0:getInvoiceNotesResponse)
     ns0:getKeyDatesForPatient(ns0:getKeyDatesForPatient)
     ns0:getKeyDatesForPatientResponse(ns0:getKeyDatesForPatientResponse)
     ns0:getOffices(ns0:getOffices)
     ns0:getOfficesResponse(ns0:getOfficesResponse)
     ns0:getOrderDetailById(ns0:getOrderDetailById)
     ns0:getOrderDetailByIdResponse(ns0:getOrderDetailByIdResponse)
     ns0:getPatientById(ns0:getPatientById)
     ns0:getPatientByIdResponse(ns0:getPatientByIdResponse)
     ns0:getPatientInsuranceInfo(ns0:getPatientInsuranceInfo)
     ns0:getPatientInsuranceInfoResponse(ns0:getPatientInsuranceInfoResponse)
     ns0:getPatientInsurancePriorities(ns0:getPatientInsurancePriorities)
     ns0:getPatientInsurancePrioritiesResponse(ns0:getPatientInsurancePrioritiesResponse)
     ns0:getPatientInsuranceTypes(ns0:getPatientInsuranceTypes)
     ns0:getPatientInsuranceTypesResponse(ns0:getPatientInsuranceTypesResponse)
     ns0:getPatientPhotoContent(ns0:getPatientPhotoContent)
     ns0:getPatientPhotoContentResponse(ns0:getPatientPhotoContentResponse)
     ns0:getPatientSchedulingPreferences(ns0:getPatientSchedulingPreferences)
     ns0:getPatientSchedulingPreferencesResponse(ns0:getPatientSchedulingPreferencesResponse)
     ns0:getProviderIdByEmployeeId(ns0:getProviderIdByEmployeeId)
     ns0:getProviderIdByEmployeeIdResponse(ns0:getProviderIdByEmployeeIdResponse)
     ns0:getProviders(ns0:getProviders)
     ns0:getProvidersResponse(ns0:getProvidersResponse)
     ns0:getRecallById(ns0:getRecallById)
     ns0:getRecallByIdResponse(ns0:getRecallByIdResponse)
     ns0:getServerTime(ns0:getServerTime)
     ns0:getServerTimeResponse(ns0:getServerTimeResponse)
     ns0:readinessCheck(ns0:readinessCheck)
     ns0:readinessCheckResponse(ns0:readinessCheckResponse)
     ns0:rescheduleAppointmentFromDetails(ns0:rescheduleAppointmentFromDetails)
     ns0:rescheduleAppointmentFromDetailsResponse(ns0:rescheduleAppointmentFromDetailsResponse)
     ns0:searchAppointmentSlots(ns0:searchAppointmentSlots)
     ns0:searchAppointmentSlotsResponse(ns0:searchAppointmentSlotsResponse)
     ns0:searchAppointments(ns0:searchAppointments)
     ns0:searchAppointmentsResponse(ns0:searchAppointmentsResponse)
     ns0:searchAppointmentsWithDetail(ns0:searchAppointmentsWithDetail)
     ns0:searchAppointmentsWithDetailResponse(ns0:searchAppointmentsWithDetailResponse)
     ns0:searchClaims(ns0:searchClaims)
     ns0:searchClaimsResponse(ns0:searchClaimsResponse)
     ns0:searchContactLensPrescriptions(ns0:searchContactLensPrescriptions)
     ns0:searchContactLensPrescriptionsResponse(ns0:searchContactLensPrescriptionsResponse)
     ns0:searchDeletedRecalls(ns0:searchDeletedRecalls)
     ns0:searchDeletedRecallsResponse(ns0:searchDeletedRecallsResponse)
     ns0:searchEncounters(ns0:searchEncounters)
     ns0:searchEncountersResponse(ns0:searchEncountersResponse)
     ns0:searchExternalMedicationPrescriptions(ns0:searchExternalMedicationPrescriptions)
     ns0:searchExternalMedicationPrescriptionsResponse(ns0:searchExternalMedicationPrescriptionsResponse)
     ns0:searchEyeglassPrescriptions(ns0:searchEyeglassPrescriptions)
     ns0:searchEyeglassPrescriptionsResponse(ns0:searchEyeglassPrescriptionsResponse)
     ns0:searchInvoicePayments(ns0:searchInvoicePayments)
     ns0:searchInvoicePaymentsResponse(ns0:searchInvoicePaymentsResponse)
     ns0:searchKeyDates(ns0:searchKeyDates)
     ns0:searchKeyDatesDetail(ns0:searchKeyDatesDetail)
     ns0:searchKeyDatesDetailResponse(ns0:searchKeyDatesDetailResponse)
     ns0:searchKeyDatesResponse(ns0:searchKeyDatesResponse)
     ns0:searchMedicationPrescriptions(ns0:searchMedicationPrescriptions)
     ns0:searchMedicationPrescriptionsResponse(ns0:searchMedicationPrescriptionsResponse)
     ns0:searchOrderDetail(ns0:searchOrderDetail)
     ns0:searchOrderDetailResponse(ns0:searchOrderDetailResponse)
     ns0:searchOrders(ns0:searchOrders)
     ns0:searchOrdersResponse(ns0:searchOrdersResponse)
     ns0:searchPatientBalances(ns0:searchPatientBalances)
     ns0:searchPatientBalancesResponse(ns0:searchPatientBalancesResponse)
     ns0:searchPatientDiagnoses(ns0:searchPatientDiagnoses)
     ns0:searchPatientDiagnosesResponse(ns0:searchPatientDiagnosesResponse)
     ns0:searchPatientInsuranceInfo(ns0:searchPatientInsuranceInfo)
     ns0:searchPatientInsuranceInfoResponse(ns0:searchPatientInsuranceInfoResponse)
     ns0:searchPatientPhotos(ns0:searchPatientPhotos)
     ns0:searchPatientPhotosResponse(ns0:searchPatientPhotosResponse)
     ns0:searchPatientTransactions(ns0:searchPatientTransactions)
     ns0:searchPatientTransactionsResponse(ns0:searchPatientTransactionsResponse)
     ns0:searchPatients(ns0:searchPatients)
     ns0:searchPatientsLimited(ns0:searchPatientsLimited)
     ns0:searchPatientsLimitedResponse(ns0:searchPatientsLimitedResponse)
     ns0:searchPatientsResponse(ns0:searchPatientsResponse)
     ns0:searchPatientsWithReferral(ns0:searchPatientsWithReferral)
     ns0:searchPatientsWithReferralResponse(ns0:searchPatientsWithReferralResponse)
     ns0:searchPaymentItems(ns0:searchPaymentItems)
     ns0:searchPaymentItemsResponse(ns0:searchPaymentItemsResponse)
     ns0:searchPaymentItemsWithLedgerPostings(ns0:searchPaymentItemsWithLedgerPostings)
     ns0:searchPaymentItemsWithLedgerPostingsResponse(ns0:searchPaymentItemsWithLedgerPostingsResponse)
     ns0:searchPayments(ns0:searchPayments)
     ns0:searchPaymentsResponse(ns0:searchPaymentsResponse)
     ns0:searchPaymentsWithLedgerPostings(ns0:searchPaymentsWithLedgerPostings)
     ns0:searchPaymentsWithLedgerPostingsResponse(ns0:searchPaymentsWithLedgerPostingsResponse)
     ns0:searchProducts(ns0:searchProducts)
     ns0:searchProductsResponse(ns0:searchProductsResponse)
     ns0:searchRecalls(ns0:searchRecalls)
     ns0:searchRecallsResponse(ns0:searchRecallsResponse)
     ns0:searchRefractions(ns0:searchRefractions)
     ns0:searchRefractionsResponse(ns0:searchRefractionsResponse)
     ns0:searchSales(ns0:searchSales)
     ns0:searchSalesResponse(ns0:searchSalesResponse)
     ns0:searchScheduleItems(ns0:searchScheduleItems)
     ns0:searchScheduleItemsResponse(ns0:searchScheduleItemsResponse)
     ns0:searchServices(ns0:searchServices)
     ns0:searchServicesResponse(ns0:searchServicesResponse)
     ns0:searchTodaysInProgressEncounters(ns0:searchTodaysInProgressEncounters)
     ns0:searchTodaysInProgressEncountersResponse(ns0:searchTodaysInProgressEncountersResponse)
     ns0:searchTransactions(ns0:searchTransactions)
     ns0:searchTransactionsResponse(ns0:searchTransactionsResponse)
     ns0:searchTransactionsV2(ns0:searchTransactionsV2)
     ns0:searchTransactionsV2Response(ns0:searchTransactionsV2Response)
     ns0:searchTransactionsWithDiagnoses(ns0:searchTransactionsWithDiagnoses)
     ns0:searchTransactionsWithDiagnosesResponse(ns0:searchTransactionsWithDiagnosesResponse)
     ns0:setPatientNotified(ns0:setPatientNotified)
     ns0:setPatientNotifiedResponse(ns0:setPatientNotifiedResponse)
     ns0:updateOrderStatus(ns0:updateOrderStatus)
     ns0:updateOrderStatusResponse(ns0:updateOrderStatusResponse)
     ns0:updatePatient(ns0:updatePatient)
     ns0:updatePatientCommunicationPreferences(ns0:updatePatientCommunicationPreferences)
     ns0:updatePatientCommunicationPreferencesResponse(ns0:updatePatientCommunicationPreferencesResponse)
     ns0:updatePatientLogin(ns0:updatePatientLogin)
     ns0:updatePatientLoginResponse(ns0:updatePatientLoginResponse)
     ns0:updatePatientResponse(ns0:updatePatientResponse)
     ns0:uploadPatientFilesToFolder(ns0:uploadPatientFilesToFolder)
     ns0:uploadPatientFilesToFolderResponse(ns0:uploadPatientFilesToFolderResponse)
     ns0:verifyPatientUserNameAvailable(ns0:verifyPatientUserNameAvailable)
     ns0:verifyPatientUserNameAvailableResponse(ns0:verifyPatientUserNameAvailableResponse)


Global types:
     xsd:anyType
     ns0:PatientInsuranceSearchRequest(pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, updatedSince: xsd:string, status: xsd:int)
     ns0:RecallSearchRequest(endDate: xsd:string, pageNumber: xsd:int, pageSize: xsd:int, startDate: xsd:string, updatedSince: xsd:string, patientId: xsd:long)
     ns0:WebServiceException(details: xsd:string, errorCode: xsd:string, errorMessage: xsd:string)
     ns0:activatePatient(patientId: xsd:long, userId: xsd:string)
     ns0:activatePatientResponse(patient: ns0:patientBasic)
     ns0:addPatient(patient: ns0:patientMinimal, userId: xsd:string)
     ns0:addPatientResponse(newPatientId: xsd:long)
     ns0:address(address1: xsd:string, address2: xsd:string, city: xsd:string, country: xsd:string, postalCode: xsd:string, stateProvince: xsd:string)
     ns0:appointmentBasic(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, appointmentId: xsd:long, apptDate: xsd:string, apptLength: xsd:int, apptNote: xsd:string, apptSubType: xsd:string, apptSubTypeId: xsd:long, apptType: xsd:string, apptTypeId: xsd:long, confirmed: xsd:boolean, lastUpdated: xsd:string, officeId: xsd:long, patientId: xsd:long, providerId: xsd:long, status: xsd:int)
     ns0:appointmentDetail(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, appointmentId: xsd:long, apptDate: xsd:string, apptLength: xsd:int, apptNote: xsd:string, apptSubType: xsd:string, apptSubTypeId: xsd:long, apptType: xsd:string, apptTypeId: xsd:long, confirmed: xsd:boolean, lastUpdated: xsd:string, officeId: xsd:long, patientId: xsd:long, providerId: xsd:long, status: xsd:int, office: ns0:office, patient: ns0:patientBasic, provider: ns0:provider)
     ns0:appointmentSearchRequest(apptStatusList: xsd:int[], apptTypeList: xsd:long[], endDate: xsd:string, officeId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, providerId: xsd:long, startDate: xsd:string, updatedSince: xsd:string)
     ns0:appointmentSlot(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, appointmentSlotId: xsd:long, 
employeeCredentials: xsd:string, employeeFirstName: xsd:string, employeeId: xsd:long, employeeLastName: xsd:string, endDate: 
xsd:string, officeId: xsd:long, officeName: xsd:string, roleId: xsd:long, roleName: xsd:string, startDate: xsd:string)       
     ns0:appointmentSlotSearchRequest(apptTypeId: xsd:long, endDate: xsd:string, officeIds: xsd:long[], pageNumber: xsd:int, 
pageSize: xsd:int, patientId: xsd:long, preferences: ns0:patientSchedulingPreferences, startDate: xsd:string)
     ns0:appointmentSubType(apptSubTypeId: xsd:long, apptSubTypeName: xsd:string)
     ns0:appointmentType(apptSubTypes: ns0:appointmentSubType[], apptTypeId: xsd:long, apptTypeName: xsd:string, duration: xsd:int)
     ns0:cancelAppointment(appointmentId: xsd:long, patientInitiated: xsd:boolean, emailPatient: xsd:boolean, reason: xsd:string, userId: xsd:string)
     ns0:cancelAppointmentResponse(result: xsd:string)
     ns0:claimSearchRequest(claimEndDate: xsd:string, claimId: xsd:long, claimProcessingMechanism: xsd:int, claimProcessingStatus: xsd:int, claimStartDate: xsd:string, claimSubmittedEndDate: xsd:string, claimSubmittedStartDate: xsd:string, insuranceCompanyId: xsd:long, invoiceEndDate: xsd:string, invoiceId: xsd:long, invoiceStartDate: xsd:string, locationId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, patientName: xsd:string, providerId: xsd:long)
     ns0:coPays(authorizationDate: xsd:string, authorizationNumber: xsd:string, contactLensAllowance: xsd:double, contactLensBenefitEligible: xsd:boolean, contactLensBenefitResetDate: xsd:string, contactLensFitting: xsd:double, contactLensFittingEligible: xsd:boolean, contactLensFittingResetDate: xsd:string, frameBenefitEligible: xsd:boolean, frameBenefitResetDate: xsd:string, lensBenefitEligible: xsd:boolean, lensBenefitResetDate: xsd:string, materials: xsd:double, maximumFrameAllowance: xsd:double, medicalExam: xsd:double, minimumFrameAllowance: xsd:double, officeVisit: xsd:double, routineExam: xsd:double, routineExamEligible: xsd:boolean, routineExamResetDate: xsd:string)
     ns0:confirmAppointment(appointmentId: xsd:long, comment: xsd:string, userId: xsd:string)
     ns0:confirmAppointmentResponse(result: xsd:string)
     ns0:contactLensPrescription(authorizationDate: xsd:dateTime, authorizationType: xsd:int, bodyLocationName: xsd:string, createdByUserName: xsd:string, createdOn: xsd:dateTime, description: xsd:string, encounterId: xsd:long, expirationDate: xsd:dateTime, externalSystemId: xsd:string, id: xsd:long, instructions: xsd:string, numRefillsAllowed: xsd:int, numRefillsRemaining: xsd:int, patientId: xsd:long, personId: xsd:long, phrEnabled: xsd:boolean, providerId: xsd:long, reason: xsd:string, startDate: xsd:dateTime, status: xsd:int, stopDate: xsd:dateTime, stopReasonId: xsd:long, updatedByUserName: xsd:string, updatedOn: xsd:dateTime, useProviderSignature: xsd:boolean, od: ns0:contactLensRxInfo, os: ns0:contactLensRxInfo)
     ns0:contactLensPrescriptionSearchRequest(authorizationType: xsd:int, endDate: xsd:string, expirationEndDate: xsd:string, expirationStartDate: xsd:string, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, providerId: xsd:long, startDate: xsd:string, status: xsd:int, updatedSince: xsd:string, contactLensTypeIds: xsd:int[])
     ns0:contactLensRxInfo(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, monovision: xsd:boolean, product: ns0:productBasic, sphere: xsd:double)
     ns0:createAppointmentBaseRequest(apptSubTypeId: xsd:long, apptTypeId: xsd:long, patientId: xsd:long)
     ns0:createAppointmentFromDetails(createAppointmentRequest: ns0:createAppointmentRequest, userId: xsd:string)
     ns0:createAppointmentFromDetailsResponse(apptId: xsd:long)
     ns0:createAppointmentFromSlot(createAppointmentFromSlotRequest: ns0:createAppointmentFromSlotRequest, userId: xsd:string)
     ns0:createAppointmentFromSlotRequest(apptSubTypeId: xsd:long, apptTypeId: xsd:long, patientId: xsd:long, appointmentSlotId: xsd:long)
     ns0:createAppointmentFromSlotResponse(apptId: xsd:long)
     ns0:createAppointmentRequest(apptSubTypeId: xsd:long, apptTypeId: xsd:long, patientId: xsd:long, description: xsd:string, employeeId: xsd:long, endDate: xsd:string, officeId: xsd:long, providerId: xsd:long, startDate: xsd:string)
     ns0:deactivatePatient(patientId: xsd:long, userId: xsd:string)
     ns0:deactivatePatientResponse(patient: ns0:patientBasic)
     ns0:deceasePatient(patientId: xsd:long, dateOfDeath: xsd:string, userId: xsd:string)
     ns0:deceasePatientResponse(patient: ns0:patientBasic)
     ns0:deletedRecall(deletedOn: xsd:string, patientId: xsd:long, recallId: xsd:long)
     ns0:echo(echoRequest: xsd:string, userId: xsd:string)
     ns0:echoResponse(echoResponse: xsd:string)
     ns0:employee(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, employeeId: xsd:long, employeePersonId: xsd:long, firstName: xsd:string, lastName: xsd:string, status: xsd:int)
     ns0:encounterBasic(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, apptSubType: xsd:string, apptSubTypeId: xsd:long, apptType: xsd:string, apptTypeId: xsd:long, encounterDate: xsd:string, encounterId: xsd:long, officeId: xsd:long, officeName: xsd:string, patientDOB: xsd:string, patientEmail: xsd:string, patientFirstName: xsd:string, patientGender: xsd:string, patientHomeAddress: ns0:address, patientHomePhone: xsd:string, patientId: xsd:long, patientLastName: xsd:string, patientMobilePhone: xsd:string, patientNickName: xsd:string, patientPreferredPhone: xsd:string, patientWorkPhone: xsd:string, providerFirstName: xsd:string, providerId: xsd:long, providerLastName: xsd:string, status: xsd:int)
     ns0:encounterSearchRequest(approvalEndDate: xsd:string, approvalStartDate: xsd:string, approvalStatus: xsd:int, employeeId: xsd:long, encounterTypeId: xsd:long, endDate: xsd:string, locationIds: xsd:long[], patientId: xsd:long, patientName: xsd:string, patientStatus: xsd:int, providerId: xsd:long, startDate: xsd:string, status: xsd:int, subTypeId: xsd:long)
     ns0:externalMedicationPrescription(authorizationDate: xsd:dateTime, authorizationType: xsd:int, bodyLocationName: xsd:string, createdByUserName: xsd:string, createdOn: xsd:dateTime, description: xsd:string, encounterId: xsd:long, expirationDate: xsd:dateTime, externalSystemId: xsd:string, id: xsd:long, instructions: xsd:string, numRefillsAllowed: xsd:int, numRefillsRemaining: xsd:int, patientId: xsd:long, personId: xsd:long, phrEnabled: xsd:boolean, providerId: xsd:long, reason: xsd:string, startDate: xsd:dateTime, status: xsd:int, stopDate: xsd:dateTime, stopReasonId: xsd:long, updatedByUserName: xsd:string, updatedOn: xsd:dateTime, useProviderSignature: xsd:boolean, dosageAmount: xsd:double, dosageUnit: xsd:string, drugBrandName: xsd:string, drugCode: xsd:string, drugCodeSet: xsd:int, drugDescription: xsd:string, drugGenericName: xsd:string, frequency: xsd:string, route: xsd:string)
     ns0:eyeglassPrescription(authorizationDate: xsd:dateTime, authorizationType: xsd:int, bodyLocationName: xsd:string, createdByUserName: xsd:string, createdOn: xsd:dateTime, description: xsd:string, encounterId: xsd:long, expirationDate: xsd:dateTime, externalSystemId: xsd:string, id: xsd:long, instructions: xsd:string, numRefillsAllowed: xsd:int, numRefillsRemaining: xsd:int, patientId: xsd:long, personId: xsd:long, phrEnabled: xsd:boolean, providerId: xsd:long, reason: xsd:string, startDate: xsd:dateTime, status: xsd:int, stopDate: xsd:dateTime, stopReasonId: xsd:long, updatedByUserName: xsd:string, updatedOn: xsd:dateTime, useProviderSignature: xsd:boolean, arCoating: xsd:boolean, arCoatingComment: xsd:string, distancePd: xsd:string, 
lensType: xsd:string, lensTypeComment: xsd:string, lensTypeId: xsd:long, material: xsd:string, materialComment: xsd:string, materialId: xsd:long, nearPd: xsd:string, odAxis: xsd:string, odBalanced: xsd:boolean, odCylinder: xsd:string, odHorizontalPrism: xsd:string, odHorizontalPrismOrientation: xsd:string, odIntermediateAdd: xsd:string, odNearAdd: xsd:string, odSphere: xsd:string, odVerticalPrism: xsd:string, odVerticalPrismOrientation: xsd:string, osAxis: xsd:string, osBalanced: xsd:boolean, osCylinder: xsd:string, osHorizontalPrism: xsd:string, osHorizontalPrismOrientation: xsd:string, osIntermediateAdd: xsd:string, osNearAdd: xsd:string, osSphere: xsd:string, osVerticalPrism: xsd:string, osVerticalPrismOrientation: xsd:string, photochromic: xsd:boolean, photochromicComment: xsd:string, polarized: xsd:boolean, polarizedComment: xsd:string, tint: xsd:string, tintComment: xsd:string, tintId: xsd:long, usedForReason: xsd:string, usedForReasonId: xsd:long, uvTreatment: xsd:boolean, uvTreatmentComment: xsd:string)
     ns0:file(contentType: xsd:string, createdOn: xsd:string, description: xsd:string, fileName: xsd:string, fileSize: xsd:long, id: xsd:long, mimeType: xsd:string, updatedOn: xsd:string)
     ns0:fileUpload(comment: xsd:string, data: xsd:base64Binary, fileName: xsd:string)
     ns0:getAccountSummaryWithInsurance(patientId: xsd:long, userId: xsd:string)
     ns0:getAccountSummaryWithInsuranceResponse(result: ns0:patientInsuranceAccountSummary)
     ns0:getAllEmployees(userId: xsd:string)
     ns0:getAllEmployeesResponse(employeeList: ns0:employee[])
     ns0:getAllProviders(userId: xsd:string)
     ns0:getAllProvidersResponse(providerList: ns0:provider[])
     ns0:getAppointmentById(appointmentId: xsd:long, userId: xsd:string)
     ns0:getAppointmentByIdResponse(appointment: ns0:appointmentBasic)
     ns0:getAppointmentDetailById(appointmentId: xsd:long, userId: xsd:string)
     ns0:getAppointmentDetailByIdResponse(appointment: ns0:appointmentDetail)
     ns0:getApptTypes(userId: xsd:string)
     ns0:getApptTypesResponse(apptTypeList: ns0:appointmentType[])
     ns0:getEmployeeIdByProviderId(providerId: xsd:long, userId: xsd:string)
     ns0:getEmployeeIdByProviderIdResponse(employeeId: xsd:long)
     ns0:getEmployeeOffices(employeeId: xsd:long, userId: xsd:string)
     ns0:getEmployeeOfficesResponse(officeList: ns0:office[])
     ns0:getEmployees(userId: xsd:string)
     ns0:getEmployeesResponse(employeeList: ns0:employee[])
     ns0:getEncounterById(encounterId: xsd:long, userId: xsd:string)
     ns0:getEncounterByIdResponse(encounterList: ns0:encounterBasic)
     ns0:getInsuranceCompanies(userId: xsd:string)
     ns0:getInsuranceCompaniesResponse(companyList: ns0:insuranceCompany[])
     ns0:getInvoiceNotes(invoiceId: xsd:long, userId: xsd:string)
     ns0:getInvoiceNotesResponse(noteList: ns0:note[])
     ns0:getKeyDatesForPatient(patientId: xsd:long, userId: xsd:string)
     ns0:getKeyDatesForPatientResponse(patient: ns0:keyDatesBasic)
     ns0:getOffices(userId: xsd:string)
     ns0:getOfficesResponse(officeList: ns0:office[])
     ns0:getOrderDetailById(orderId: xsd:long, userId: xsd:string)
     ns0:getOrderDetailByIdResponse(order: ns0:orderDetail)
     ns0:getPatientById(patientId: xsd:long, userId: xsd:string)
     ns0:getPatientByIdResponse(patient: ns0:patientBasic)
     ns0:getPatientInsuranceInfo(patientId: xsd:long, userId: xsd:string)
     ns0:getPatientInsuranceInfoResponse(insuranceInfo: ns0:insurance[])
     ns0:getPatientInsurancePriorities(userId: xsd:string)
     ns0:getPatientInsurancePrioritiesResponse(insurancePriority: ns0:insurancePriority[])
     ns0:getPatientInsuranceTypes(userId: xsd:string)
     ns0:getPatientInsuranceTypesResponse(insuranceType: ns0:insuranceType[])
     ns0:getPatientPhotoContent(patientPhotoId: xsd:long, userId: xsd:string)
     ns0:getPatientPhotoContentResponse(return: xsd:base64Binary)
     ns0:getPatientSchedulingPreferences(patientId: xsd:long, userId: xsd:string)
     ns0:getPatientSchedulingPreferencesResponse(patientSchedulingPreferences: ns0:patientSchedulingPreferences)
     ns0:getProviderIdByEmployeeId(employeeId: xsd:long, userId: xsd:string)
     ns0:getProviderIdByEmployeeIdResponse(providerId: xsd:long)
     ns0:getProviders(userId: xsd:string)
     ns0:getProvidersResponse(providerList: ns0:provider[])
     ns0:getRecallById(recallId: xsd:long, userId: xsd:string)
     ns0:getRecallByIdResponse(recall: ns0:recallBasic)
     ns0:getServerTime(userId: xsd:string)
     ns0:getServerTimeResponse(currentServerTime: xsd:string)
     ns0:hybridContactLensRxInfo(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: 
xsd:double, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, monovision: xsd:boolean, 
product: ns0:productBasic, sphere: xsd:double, addZoneSize: xsd:string, design: xsd:string, segmentSize: xsd:string, skirtCurveRadius: xsd:string, vault: xsd:int)
     ns0:insurance(copays: ns0:coPays, groupNumber: xsd:string, id: xsd:long, individualCopays: ns0:coPays, insuranceCompanyName: xsd:string, insuranceType: xsd:string, patientId: xsd:long, policyNumber: xsd:string, priority: xsd:string)
     ns0:insuranceClaim(claimDate: xsd:string, claimSubmissionMechanism: xsd:int, claimSubmitDate: xsd:string, externalId: xsd:string, externalMessage: xsd:string, id: xsd:long, insuranceClaimProcessorName: xsd:string, invoiceId: xsd:long, patientId: xsd:long, processingStatus: xsd:int, status: xsd:int)
     ns0:insuranceCompany(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, companyId: xsd:long, name: xsd:string, payorId: xsd:string, status: xsd:int)
     ns0:insurancePriority(active: xsd:boolean, description: xsd:string, id: xsd:long, name: xsd:string)
     ns0:insuranceType(active: xsd:boolean, description: xsd:string, id: xsd:long, name: xsd:string)
     ns0:keyDatesBasic(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, lastCompExamDate: xsd:string, lastCompExamId: xsd:long, lastCompExamProviderId: xsd:long, lastCompExamRefreshDate: xsd:string, lastCompExamType: xsd:string, lastExamDate: xsd:string, lastExamId: xsd:long, lastExamProviderId: xsd:long, lastExamRefreshDate: xsd:string, lastExamType: xsd:string, nextApptDate: xsd:string, nextApptId: xsd:long, nextApptProviderId: xsd:long, nextApptRefreshDate: xsd:string, nextApptType: xsd:string, nextRecallDate: xsd:string, nextRecallId: xsd:long, nextRecallRefreshDate: xsd:string, nextRecallType: xsd:string, patientId: xsd:long)
     ns0:keyDatesDetail(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, lastCompExamDate: xsd:string, 
lastCompExamId: xsd:long, lastCompExamProviderId: xsd:long, lastCompExamRefreshDate: xsd:string, lastCompExamType: xsd:string, lastExamDate: xsd:string, lastExamId: xsd:long, lastExamProviderId: xsd:long, lastExamRefreshDate: xsd:string, lastExamType: xsd:string, nextApptDate: xsd:string, nextApptId: xsd:long, nextApptProviderId: xsd:long, nextApptRefreshDate: xsd:string, 
nextApptType: xsd:string, nextRecallDate: xsd:string, nextRecallId: xsd:long, nextRecallRefreshDate: xsd:string, nextRecallType: xsd:string, patientId: xsd:long, patient: ns0:patientBasic)
     ns0:keyDatesSearchRequest(endDate: xsd:string, keyDateType: xsd:int, officeId: xsd:long, pageNumber: xsd:int, pageSize: 
xsd:int, startDate: xsd:string, updatedSince: xsd:string)
     ns0:ledgerPosting(amount: xsd:double, details: xsd:string, id: xsd:long, postedOn: xsd:string, quantityChange: xsd:int, 
taxAmount: xsd:double)
     ns0:limitedPatientSearchRequest(activeOnly: xsd:boolean, dob: xsd:string, firstName: xsd:string, lastName: xsd:string, officeId: xsd:long, patientId: xsd:long)
     ns0:medicationPrescription(authorizationDate: xsd:dateTime, authorizationType: xsd:int, bodyLocationName: xsd:string, createdByUserName: xsd:string, createdOn: xsd:dateTime, description: xsd:string, encounterId: xsd:long, expirationDate: xsd:dateTime, externalSystemId: xsd:string, id: xsd:long, instructions: xsd:string, numRefillsAllowed: xsd:int, numRefillsRemaining: xsd:int, patientId: xsd:long, personId: xsd:long, phrEnabled: xsd:boolean, providerId: xsd:long, reason: xsd:string, startDate: xsd:dateTime, status: xsd:int, stopDate: xsd:dateTime, stopReasonId: xsd:long, updatedByUserName: xsd:string, updatedOn: 
xsd:dateTime, useProviderSignature: xsd:boolean, dosageAmount: xsd:double, dosageUnit: xsd:string, drugBrandName: xsd:string, drugCode: xsd:string, drugCodeSet: xsd:int, drugDescription: xsd:string, drugGenericName: xsd:string, frequency: xsd:string, route: xsd:string)
     ns0:note(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, categoryId: xsd:long, createdBy: xsd:string, createdOn: xsd:string, entityId: xsd:string, id: xsd:long, parentId: xsd:long, status: xsd:int, subCategoryId: xsd:long, text: xsd:string, user: xsd:string)
     ns0:office(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, address: ns0:address, name: xsd:string, officeId: xsd:long, storeNumber: xsd:string)
     ns0:orderBasic(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, comment: xsd:string, createdOn: xsd:string, instructions: xsd:string, lastUpdated: xsd:string, officeId: xsd:long, orderId: xsd:long, orderType: xsd:int, patientId: xsd:long, patientNotified: xsd:boolean, shipToType: xsd:int, statusCode: xsd:int, statusDate: xsd:string, statusName: xsd:string, vendorName: xsd:string)
     ns0:orderDetail(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, comment: xsd:string, createdOn: xsd:string, instructions: xsd:string, lastUpdated: xsd:string, officeId: xsd:long, orderId: xsd:long, orderType: xsd:int, patientId: xsd:long, patientNotified: xsd:boolean, shipToType: xsd:int, statusCode: xsd:int, statusDate: xsd:string, statusName: 
xsd:string, vendorName: xsd:string)
     ns0:orderDetailContactLens(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, comment: xsd:string, createdOn: xsd:string, instructions: xsd:string, lastUpdated: xsd:string, officeId: xsd:long, orderId: xsd:long, orderType: xsd:int, patientId: xsd:long, patientNotified: xsd:boolean, shipToType: xsd:int, statusCode: xsd:int, statusDate: xsd:string, statusName: xsd:string, vendorName: xsd:string, lensType: xsd:int, odLensRx: ns0:orderDetailContactLensRx, osLensRx: ns0:orderDetailContactLensRx, quantityOd: xsd:int, quantityOs: xsd:int, unitOd: xsd:string, unitOs: xsd:string, prescription: ns0:prescription)
     ns0:orderDetailContactLensRx(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, isMonovision: xsd:boolean, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, product: ns0:productBasic, sphere: xsd:double)
     ns0:orderDetailEyeglasses(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, comment: xsd:string, createdOn: xsd:string, instructions: xsd:string, lastUpdated: xsd:string, officeId: xsd:long, orderId: xsd:long, orderType: xsd:int, patientId: xsd:long, patientNotified: xsd:boolean, shipToType: xsd:int, statusCode: xsd:int, statusDate: xsd:string, statusName: xsd:string, vendorName: xsd:string, binocularPdDistance: xsd:double, binocularPdNear: xsd:double, frameIndication: 
xsd:int, frameInfo: ns0:orderDetailFrameInfo, frameProduct: ns0:productBasic, lensRequest: xsd:int, odLens: ns0:orderDetailLens, options: ns0:orderDetailOption[], osLens: ns0:orderDetailLens, panto: xsd:double, polishEdges: xsd:boolean, prescription: ns0:orderDetailEyeglassesRx, quantity: xsd:int, rollEdges: xsd:boolean, wrapAngle: xsd:double, odLensProduct: ns0:productBasic, osLensProduct: ns0:productBasic)
     ns0:orderDetailEyeglassesRx(binocularPdDistance: xsd:double, binocularPdNear: xsd:double, odLensRx: ns0:orderDetailLensRx, osLensRx: ns0:orderDetailLensRx)
     ns0:orderDetailFrame(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, comment: xsd:string, createdOn: xsd:string, instructions: xsd:string, lastUpdated: xsd:string, officeId: xsd:long, orderId: xsd:long, orderType: xsd:int, patientId: xsd:long, patientNotified: xsd:boolean, shipToType: xsd:int, statusCode: xsd:int, statusDate: xsd:string, statusName: xsd:string, vendorName: xsd:string, frameInfo: ns0:orderDetailFrameInfo, product: ns0:productBasic, quantity: xsd:int)  
     ns0:orderDetailFrameInfo(a: xsd:double, b: xsd:double, bridge: xsd:double, circumference: xsd:double, colorCode: xsd:string, colorName: xsd:string, dbl: xsd:double, ed: xsd:double, edAngle: xsd:double, eye: xsd:double, genericColorName: xsd:string, lensColorCode: xsd:string, lensColorName: xsd:string, screwToScrew: xsd:double, temple: xsd:double, templeUnit: xsd:string)
     ns0:orderDetailHybridContactLensRx(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, isMonovision: xsd:boolean, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, product: ns0:productBasic, sphere: xsd:double, addZoneSize: xsd:string, design: xsd:string, segmentSize: xsd:string, skirtCurveRadius: xsd:string, vault: xsd:int)
     ns0:orderDetailLens(backVertexDistance: xsd:double, baseCurve: xsd:double, blankSize: xsd:double, monocularPd: xsd:double, monocularPdNear: xsd:double, opticalCenter: xsd:double, opticalCenterType: xsd:int, segHeight: xsd:double, segHeightType: 
xsd:int)
     ns0:orderDetailLensRx(axis: xsd:int, balanced: xsd:boolean, cylinder: xsd:double, horizontalPrism: xsd:double, horizontalPrismOrientation: xsd:string, intermediateAdd: xsd:double, nearAdd: xsd:double, sphere: xsd:double, verticalPrism: xsd:double, verticalPrismOrientation: xsd:string)
     ns0:orderDetailOption(categoryId: xsd:int, name: xsd:string, product: ns0:productBasic, value: xsd:string)
     ns0:orderDetailRigidContactLensRx(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, isMonovision: xsd:boolean, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, product: ns0:productBasic, sphere: xsd:double, addDiameter: xsd:double, backOpticalDiameter: xsd:double, baseCurve2: 
xsd:double, bcUnit: xsd:string, centerThickness: xsd:double, distanceZone: xsd:double, dot: xsd:boolean, edgeLift: xsd:string, edgeLiftAmount: xsd:double, fenestration: xsd:boolean, firstCurveRadius: xsd:double, firstCurveWidth: xsd:double, fourthCurveRadius: xsd:double, fourthCurveWidth: xsd:double, intermediateSegment: xsd:double, landingZoneAngle: xsd:int, lensMaterial: xsd:string, midPeripheralLimbalClearance: xsd:string, notes: xsd:string, opticZone: xsd:double, peripheralCurveRadius: xsd:double, peripheralCurveWidth: xsd:double, peripheralEdge: xsd:string, plasmaTreatment: xsd:boolean, profile: xsd:string, returnZoneDiameter: xsd:int, sagittalDepth: xsd:double, secondCurveRadius: xsd:double, secondCurveWidth: xsd:double, secondaryCurveRadius: xsd:double, secondaryCurveWidth: xsd:double, segmentHeight: xsd:double, specialCharacteristics: xsd:string, sphere2: xsd:double, thirdCurveRadius: xsd:double, thirdCurveWidth: xsd:double, truncation: xsd:double)
     ns0:orderDetailSoftContactLensRx(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, isMonovision: xsd:boolean, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, product: ns0:productBasic, sphere: xsd:double, addDesignation: xsd:string)
     ns0:orderNotificationStatusUpdateRequest(notificationComments: xsd:string, notifiedDate: xsd:string, orderId: xsd:long) 
     ns0:orderSearchRequest(endDate: xsd:string, locationId: xsd:long, masterProcessorId: xsd:long, notNotifiedOnly: xsd:boolean, orderId: xsd:long, orderType: xsd:int, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, shipToType: xsd:int, startDate: xsd:string, statusCode: xsd:int, statusList: xsd:int[], updatedSince: xsd:string, vendorName: xsd:string)        
     ns0:orderStatusUpdateRequest(comment: xsd:string, newStatus: xsd:int, orderId: xsd:long)
     ns0:patientAccountSummary(balance: xsd:double, credit: xsd:double)
     ns0:patientBalance(balance: xsd:double, credit: xsd:double, patientId: xsd:long, updatedDate: xsd:string)
     ns0:patientBalanceSearchRequest(hasBalance: xsd:boolean, locationId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, updatedSince: xsd:string)
     ns0:patientBasic(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, address: ns0:address, cellPhone: xsd:string, commApptMask: xsd:int, commApptOptIn: xsd:int, commGeneralMask: xsd:int, commGeneralOptIn: xsd:int, commOrderMask: xsd:int, commOrderOptIn: xsd:int, commRecallMask: xsd:int, commRecallOptIn: xsd:int, credentials: xsd:string, dob: xsd:string, email: xsd:string, familyAccountId: xsd:long, firstName: xsd:string, gender: xsd:string, guarantorAddress: ns0:address, 
guarantorCellPhone: xsd:string, guarantorCellPhoneExt: xsd:string, guarantorCredentials: xsd:string, guarantorEmail: xsd:string, guarantorFirstName: xsd:string, guarantorHomePhone: xsd:string, guarantorHomePhoneExt: xsd:string, guarantorId: xsd:long, guarantorLastName: xsd:string, guarantorMiddleName: xsd:string, guarantorNickName: xsd:string, guarantorSuffix: xsd:string, 
guarantorWorkPhone: xsd:string, guarantorWorkPhoneExt: xsd:string, headOfHousehold: xsd:boolean, homePhone: xsd:string, lastName: xsd:string, lastUpdated: xsd:string, maskedSsn: xsd:string, middleName: xsd:string, nickName: xsd:string, patientId: xsd:long, preferredPhoneNumber: xsd:string, primaryLocationId: xsd:long, primaryProviderId: xsd:long, startDate: xsd:string, status: xsd:string, suffix: xsd:string, workPhone: xsd:string, workPhoneExt: xsd:string, commOptOutMask: xsd:int)
     ns0:patientCommunicationPreferenceUpdate(changeMask: xsd:int, doChangeOptIn: xsd:boolean, mask: xsd:int, optIn: xsd:int, preferenceType: xsd:int)
     ns0:patientDiagnosis(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, assessedDate: xsd:string, codeSet: xsd:string, comment: xsd:string, createdDate: xsd:string, diagnosisCode: xsd:string, diagnosisDate: xsd:string, encounterId: xsd:long, isMasterDiagnosis: xsd:boolean, isPrimary: xsd:boolean, location: xsd:string, longDescription: xsd:string, patientDiagnosisId: xsd:long, patientId: xsd:long, personId: xsd:long, qualifier: xsd:string, reason: xsd:string, resolutionDate: xsd:string, shortDescription: xsd:string, status: xsd:string, updatedDate: xsd:string)
     ns0:patientDiagnosisSearchRequest(codeSet: xsd:string, diagnosisCodes: xsd:string[], diagnosisDateEnd: xsd:string, diagnosisDateStart: xsd:string, pageNumber: xsd:int, pageSize: xsd:int, resolutionDateEnd: xsd:string, resolutionDateStart: xsd:string, searchMaster: xsd:boolean, status: xsd:string, updatedSinceDate: xsd:string)
     ns0:patientFamilyAccountSummary(familyBalance: xsd:double, familyCollections: xsd:double, familyCredit: xsd:double)     
     ns0:patientFile(file: ns0:file, id: xsd:long, patientId: xsd:long)
     ns0:patientInsurance(coPays: ns0:coPays, createdOn: xsd:string, deductible: xsd:double, id: xsd:long, insuranceType: xsd:long, patientBenefits: xsd:string, patientId: xsd:long, policy: ns0:patientInsurancePolicy, policyHolderRelationship: xsd:int, policyNumber: xsd:string, priorityId: xsd:long, status: xsd:int, updatedOn: xsd:string)
     ns0:patientInsuranceAccountSummary(balance: xsd:double, credit: xsd:double, collectionsBalance: xsd:double, family: ns0:patientFamilyAccountSummary, insBalance: xsd:double)
     ns0:patientInsurancePolicy(coInsurancePct: xsd:double, coPays: ns0:coPays, effectiveDate: xsd:string, familyDeductible: 
xsd:double, feeScheduleId: xsd:long, groupNumber: xsd:string, id: xsd:long, insCompanyId: xsd:long, planName: xsd:string, policyBenefits: xsd:string, policyHolderPatientId: xsd:long, referralRequired: xsd:boolean, rxBinNumber: xsd:string, rxPcnNumber: xsd:string, status: xsd:int, tpaId: xsd:long)
     ns0:patientLogin(newPassword: xsd:string, oldPassword: xsd:string, patientId: xsd:long, userName: xsd:string)
     ns0:patientMinimal(address: ns0:address, cellPhone: xsd:string, credentials: xsd:string, dob: xsd:string, email: xsd:string, firstName: xsd:string, gender: xsd:string, homePhone: xsd:string, lastName: xsd:string, middleName: xsd:string, nickName: xsd:string, patientId: xsd:long, preferredPhoneNumber: xsd:string, primaryLocationId: xsd:long, primaryProviderId: xsd:long, suffix: xsd:string, workPhone: xsd:string, workPhoneExt: xsd:string)
     ns0:patientPhoto(file: ns0:file, id: xsd:long, practiceId: xsd:long, patientId: xsd:long)
     ns0:patientPhotoSearchRequest(patientId: xsd:long, updatedSince: xsd:string)
     ns0:patientReferral(comments: xsd:string, referralDate: xsd:string, referringPatient: ns0:patientBasic, referringProvider: ns0:provider, rewardDate: xsd:string, rewardProgram: xsd:string, sourceName: xsd:string, sourceType: xsd:int)
     ns0:patientSchedulingPreferences(apptReminderType: xsd:int, fridayPreferredTime: xsd:int, mondayPreferredTime: xsd:int, 
saturdayPreferredTime: xsd:int, sundayPreferredTime: xsd:int, thursdayPreferredTime: xsd:int, tuesdayPreferredTime: xsd:int, 
wednesdayPreferredTime: xsd:int)
     ns0:patientSearchRequest(activeOnly: xsd:boolean, dob: xsd:string, firstName: xsd:string, lastName: xsd:string, officeId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, phone: xsd:string, updatedSince: xsd:string)        
     ns0:patientWithReferral(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, address: ns0:address, cellPhone: xsd:string, commApptMask: xsd:int, commApptOptIn: xsd:int, commGeneralMask: xsd:int, commGeneralOptIn: xsd:int, commOrderMask: xsd:int, commOrderOptIn: xsd:int, commRecallMask: xsd:int, commRecallOptIn: xsd:int, credentials: xsd:string, dob: 
xsd:string, email: xsd:string, familyAccountId: xsd:long, firstName: xsd:string, gender: xsd:string, guarantorAddress: ns0:address, guarantorCellPhone: xsd:string, guarantorCellPhoneExt: xsd:string, guarantorCredentials: xsd:string, guarantorEmail: xsd:string, guarantorFirstName: xsd:string, guarantorHomePhone: xsd:string, guarantorHomePhoneExt: xsd:string, guarantorId: xsd:long, guarantorLastName: xsd:string, guarantorMiddleName: xsd:string, guarantorNickName: xsd:string, guarantorSuffix: xsd:string, guarantorWorkPhone: xsd:string, guarantorWorkPhoneExt: xsd:string, headOfHousehold: xsd:boolean, homePhone: xsd:string, lastName: xsd:string, lastUpdated: xsd:string, maskedSsn: xsd:string, middleName: xsd:string, nickName: xsd:string, patientId: xsd:long, preferredPhoneNumber: xsd:string, primaryLocationId: xsd:long, primaryProviderId: xsd:long, startDate: xsd:string, status: xsd:string, suffix: xsd:string, workPhone: xsd:string, workPhoneExt: xsd:string, commOptOutMask: xsd:int, referral: ns0:patientReferral)
     ns0:payment(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, amount: xsd:double, cardType: xsd:int, comment: xsd:string, invoiceId: xsd:long, invoiceItemId: xsd:long, paymentDate: xsd:string, paymentId: xsd:long, paymentMethod: xsd:int, payor: ns0:payor, referenceNumber: xsd:string, status: xsd:int)
     ns0:paymentDatesExtendedSearchRequest(endDate: xsd:string, officeId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, startDate: xsd:string, payorType: xsd:int, postEndDate: xsd:string, postStartDate: xsd:string)
     ns0:paymentExtendedSearchRequest(endDate: xsd:string, officeId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, startDate: xsd:string, payorType: xsd:int)
     ns0:paymentSearchRequest(endDate: xsd:string, officeId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, startDate: xsd:string)
     ns0:paymentWithLedgerPostings(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, amount: xsd:double, cardType: xsd:int, comment: xsd:string, invoiceId: xsd:long, invoiceItemId: xsd:long, paymentDate: xsd:string, paymentId: xsd:long, paymentMethod: xsd:int, payor: ns0:payor, referenceNumber: xsd:string, status: xsd:int, ledgerPostings: ns0:ledgerPosting[])
     ns0:payor(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, firstName: xsd:string, lastName: xsd:string, name: xsd:string, payorId: xsd:long, type: xsd:int)
     ns0:practiceFile(file: ns0:file, id: xsd:long, practiceId: xsd:long)
     ns0:prescription(authorizationDate: xsd:dateTime, authorizationType: xsd:int, bodyLocationName: xsd:string, createdByUserName: xsd:string, createdOn: xsd:dateTime, description: xsd:string, encounterId: xsd:long, expirationDate: xsd:dateTime, externalSystemId: xsd:string, id: xsd:long, instructions: xsd:string, numRefillsAllowed: xsd:int, numRefillsRemaining: xsd:int, 
patientId: xsd:long, personId: xsd:long, phrEnabled: xsd:boolean, providerId: xsd:long, reason: xsd:string, startDate: xsd:dateTime, status: xsd:int, stopDate: xsd:dateTime, stopReasonId: xsd:long, updatedByUserName: xsd:string, updatedOn: xsd:dateTime, useProviderSignature: xsd:boolean)
     ns0:prescriptionSearchRequest(authorizationType: xsd:int, endDate: xsd:string, expirationEndDate: xsd:string, expirationStartDate: xsd:string, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, providerId: xsd:long, startDate: xsd:string, status: xsd:int, updatedSince: xsd:string)
     ns0:productBasic(active: xsd:boolean, actualCost: xsd:double, additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, brandId: xsd:long, brandName: xsd:string, categoryId: xsd:long, categoryName: xsd:string, collectionId: xsd:long, collectionName: xsd:string, description: xsd:string, discontinued: xsd:boolean, locationProductId: xsd:long, manufacturerId: xsd:long, manufacturerName: xsd:string, master: xsd:boolean, multiplier: xsd:double, name: xsd:string, productCode: xsd:string, productId: xsd:long, retailPrice: xsd:double, sku: xsd:string, upc: xsd:string, wholesalePrice: xsd:double)
     ns0:productSearchRequest(activeOnly: xsd:boolean, category: xsd:long, categoryList: xsd:long[], locationId: xsd:long, locationProductId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, updatedSince: xsd:string)
     ns0:provider(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, firstName: xsd:string, lastName: xsd:string, npi: xsd:string, providerId: xsd:long, providerType: xsd:int, status: xsd:int)
     ns0:readinessCheck()
     ns0:readinessCheckResponse()
     ns0:recallBasic(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, appointmentId: xsd:long, lastUpdated: xsd:string, patientId: xsd:long, recallComments: xsd:string, recallDate: xsd:string, recallId: xsd:long, recallReason: xsd:string, status: xsd:int)
     ns0:refraction(addVisualAcuity: xsd:string, addVisualAcuityModifier: xsd:string, comment: xsd:string, encounterId: xsd:long, instructions: xsd:string, name: xsd:string, od: ns0:refractionEye, os: ns0:refractionEye, ouVisualAcuity: xsd:string, ouVisualAcuityModifier: xsd:string, testDate: xsd:string)
     ns0:refractionEye(axis: xsd:string, balanced: xsd:boolean, cylinder: xsd:string, horizontalPrism: xsd:string, horizontalPrismOrientation: xsd:string, intermediateAdd: xsd:string, nearAdd: xsd:string, prism: xsd:string, prismOrientation: xsd:string, sphere: xsd:string, visualAcuity: xsd:string, visualAcuityModifier: xsd:string)
     ns0:refractionSearchRequest(encounterId: xsd:long, endDate: xsd:dateTime, masterIds: xsd:int[], patientId: xsd:long, startDate: xsd:dateTime)
     ns0:rescheduleAppointmentFromDetails(rescheduleAppointmentRequest: ns0:rescheduleAppointmentRequest, userId: xsd:string)     ns0:rescheduleAppointmentFromDetailsResponse(apptId: xsd:long)
     ns0:rescheduleAppointmentRequest(appointmentId: xsd:long, isCopyInsVerification: xsd:boolean, isEmailPatient: xsd:boolean, isPatientInitiated: xsd:boolean, newAppointment: ns0:createAppointmentRequest, reason: xsd:string)
     ns0:rigidContactLensRxInfo(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, monovision: xsd:boolean, product: ns0:productBasic, sphere: xsd:double, addDiameter: xsd:double, backOpticalDiameter: xsd:double, baseCurve2: xsd:double, bcUnit: xsd:string, centerThickness: xsd:double, distanceZone: xsd:double, dot: xsd:boolean, edgeLift: xsd:string, edgeLiftAmount: xsd:double, fenestration: xsd:boolean, firstCurveRadius: xsd:double, firstCurveWidth: xsd:double, fourthCurveRadius: xsd:double, fourthCurveWidth: xsd:double, intermediateSegment: xsd:double, landingZoneAngle: xsd:int, lensMaterial: xsd:string, midPeripheralLimbalClearance: xsd:string, notes: xsd:string, opticZone: xsd:double, peripheralCurveRadius: xsd:double, peripheralCurveWidth: xsd:double, peripheralEdge: xsd:string, plasmaTreatment: xsd:boolean, profile: xsd:string, returnZoneDiameter: xsd:int, sagittalDepth: xsd:double, secondCurveRadius: xsd:double, secondCurveWidth: xsd:double, secondaryCurveRadius: 
xsd:double, secondaryCurveWidth: xsd:double, segmentHeight: xsd:double, specialCharacteristics: xsd:string, sphere2: xsd:double, thirdCurveRadius: xsd:double, thirdCurveWidth: xsd:double, truncation: xsd:double)
     ns0:salesItem(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, adjustmentId: xsd:long, adjustmentType: xsd:int, adjustmentTypeString: xsd:string, adjustments: xsd:double, brandId: xsd:long, brandName: xsd:string, categoryId: xsd:long, categoryName: xsd:string, collectionId: xsd:long, collectionName: xsd:string, discounts: xsd:double, gross: xsd:double, invoiceId: xsd:long, itemCode: xsd:string, itemDescription: xsd:string, itemId: xsd:long, itemTaxId: xsd:long, itemTaxName: xsd:string, itemType: xsd:int, itemTypeString: xsd:string, manufacturerId: xsd:long, manufacturerName: xsd:string, net: xsd:double, officeId: xsd:long, orderId: xsd:long, patientFirstName: xsd:string, patientId: xsd:long, patientLastName: xsd:string, payorEntityId: xsd:long, payorId: xsd:long, payorName: xsd:string, payorType: xsd:int, payorTypeString: xsd:string, postedOn: xsd:string, practiceId: xsd:long, productId: xsd:long, productUPC: xsd:string, providerId: xsd:long, providerName: xsd:string, quantity: xsd:int, respPersonFirstName: xsd:string, respPersonId: xsd:long, respPersonLastName: xsd:string, serviceDate: xsd:string, serviceId: xsd:long, taxes: xsd:double)
     ns0:salesSearchRequest(endDate: xsd:string, invoiceId: xsd:long, itemTypes: xsd:int[], officeIds: xsd:long[], pageNumber: xsd:int, pageSize: xsd:int, patientIds: xsd:long[], payorInsuranceId: xsd:long, payorPatientId: xsd:long, payorType: xsd:int, productCategoryIds: xsd:long[], productIds: xsd:long[], providerIds: xsd:long[], serviceIds: xsd:long[], startDate: xsd:string)
     ns0:scheduleItem(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, appointmentId: xsd:long, createdOn: xsd:string, description: xsd:string, duration: xsd:int, employeeId: xsd:long, endDate: xsd:string, isRecurring: xsd:boolean, officeId: xsd:long, patientId: xsd:long, roleId: xsd:long, roleName: xsd:string, scheduleItemId: xsd:long, startDate: xsd:string, status: xsd:int, summary: xsd:string, type: xsd:int, updatedOn: xsd:string)
     ns0:scheduleItemSearchRequest(employeeIds: xsd:long[], endDate: xsd:string, itemIds: xsd:long[], itemStatuses: xsd:int[], itemTypes: xsd:int[], officeId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, startDate: xsd:string, updatedSince: xsd:string)
     ns0:searchAppointmentSlots(searchRequest: ns0:appointmentSlotSearchRequest, userId: xsd:string)
     ns0:searchAppointmentSlotsResponse(appointmentSlotList: ns0:appointmentSlot[])
     ns0:searchAppointments(searchRequest: ns0:appointmentSearchRequest, userId: xsd:string)
     ns0:searchAppointmentsResponse(appointmentList: ns0:appointmentBasic[])
     ns0:searchAppointmentsWithDetail(searchRequest: ns0:appointmentSearchRequest, userId: xsd:string)
     ns0:searchAppointmentsWithDetailResponse(appointmentList: ns0:appointmentDetail[])
     ns0:searchClaims(searchRequest: ns0:claimSearchRequest, userId: xsd:string)
     ns0:searchClaimsResponse(claims: ns0:insuranceClaim[])
     ns0:searchContactLensPrescriptions(searchRequest: ns0:contactLensPrescriptionSearchRequest, userId: xsd:string)
     ns0:searchContactLensPrescriptionsResponse(contactLensPrescriptionList: ns0:contactLensPrescription[])
     ns0:searchDeletedRecalls(searchRequest: ns0:RecallSearchRequest, userId: xsd:string)
     ns0:searchDeletedRecallsResponse(deletedRecallList: ns0:deletedRecall[])
     ns0:searchEncounters(searchRequest: ns0:encounterSearchRequest, userId: xsd:string)
     ns0:searchEncountersResponse(encounterList: ns0:encounterBasic[])
     ns0:searchExternalMedicationPrescriptions(searchRequest: ns0:prescriptionSearchRequest, userId: xsd:string)
     ns0:searchExternalMedicationPrescriptionsResponse(medicationPrescription: ns0:medicationPrescription[])
     ns0:searchEyeglassPrescriptions(searchRequest: ns0:prescriptionSearchRequest, userId: xsd:string)
     ns0:searchEyeglassPrescriptionsResponse(eyeglassPrescriptionList: ns0:eyeglassPrescription[])
     ns0:searchInvoicePayments(searchRequest: ns0:paymentSearchRequest, userId: xsd:string)
     ns0:searchInvoicePaymentsResponse(paymentList: ns0:payment[])
     ns0:searchKeyDates(searchRequest: ns0:keyDatesSearchRequest, userId: xsd:string)
     ns0:searchKeyDatesDetail(searchRequest: ns0:keyDatesSearchRequest, userId: xsd:string)
     ns0:searchKeyDatesDetailResponse(return: ns0:keyDatesDetail[])
     ns0:searchKeyDatesResponse(keyDateList: ns0:keyDatesBasic[])
     ns0:searchMedicationPrescriptions(searchRequest: ns0:prescriptionSearchRequest, userId: xsd:string)
     ns0:searchMedicationPrescriptionsResponse(medicationPrescription: ns0:medicationPrescription[])
     ns0:searchOrderDetail(searchRequest: ns0:orderSearchRequest, userId: xsd:string)
     ns0:searchOrderDetailResponse(orderDetailList: ns0:orderDetail[])
     ns0:searchOrders(searchRequest: ns0:orderSearchRequest, userId: xsd:string)
     ns0:searchOrdersResponse(orderList: ns0:orderBasic[])
     ns0:searchPatientBalances(patientId: ns0:patientBalanceSearchRequest, userId: xsd:string)
     ns0:searchPatientBalancesResponse(patientBalanceList: ns0:patientBalance[])
     ns0:searchPatientDiagnoses(searchRequest: ns0:patientDiagnosisSearchRequest, userId: xsd:string)
     ns0:searchPatientDiagnosesResponse(patientDiagnosisList: ns0:patientDiagnosis[])
     ns0:searchPatientInsuranceInfo(searchRequest: ns0:PatientInsuranceSearchRequest, userId: xsd:string)
     ns0:searchPatientInsuranceInfoResponse(insuranceInfo: ns0:patientInsurance[])
     ns0:searchPatientPhotos(searchRequest: ns0:patientPhotoSearchRequest, userId: xsd:string)
     ns0:searchPatientPhotosResponse(patientPhoto: ns0:patientPhoto[])
     ns0:searchPatientTransactions(searchRequest: ns0:transactionSearchRequest, userId: xsd:string)
     ns0:searchPatientTransactionsResponse(transactionList: ns0:transaction[])
     ns0:searchPatients(searchRequest: ns0:patientSearchRequest, userId: xsd:string)
     ns0:searchPatientsLimited(searchRequest: ns0:limitedPatientSearchRequest, userId: xsd:string)
     ns0:searchPatientsLimitedResponse(patientList: ns0:patientBasic[])
     ns0:searchPatientsResponse(patientList: ns0:patientBasic[])
     ns0:searchPatientsWithReferral(searchRequest: ns0:patientSearchRequest, userId: xsd:string)
     ns0:searchPatientsWithReferralResponse(patientList: ns0:patientWithReferral[])
     ns0:searchPaymentItems(searchRequest: ns0:paymentExtendedSearchRequest, userId: xsd:string)
     ns0:searchPaymentItemsResponse(paymentList: ns0:payment[])
     ns0:searchPaymentItemsWithLedgerPostings(searchRequest: ns0:paymentDatesExtendedSearchRequest, userId: xsd:string)      
     ns0:searchPaymentItemsWithLedgerPostingsResponse(paymentList: ns0:paymentWithLedgerPostings[])
     ns0:searchPayments(searchRequest: ns0:paymentExtendedSearchRequest, userId: xsd:string)
     ns0:searchPaymentsResponse(paymentList: ns0:payment[])
     ns0:searchPaymentsWithLedgerPostings(searchRequest: ns0:paymentDatesExtendedSearchRequest, userId: xsd:string)
     ns0:searchPaymentsWithLedgerPostingsResponse(paymentList: ns0:paymentWithLedgerPostings[])
     ns0:searchProducts(searchRequest: ns0:productSearchRequest, userId: xsd:string)
     ns0:searchProductsResponse(productList: ns0:productBasic[])
     ns0:searchRecalls(searchRequest: ns0:RecallSearchRequest, userId: xsd:string)
     ns0:searchRecallsResponse(recallList: ns0:recallBasic[])
     ns0:searchRefractions(searchRequest: ns0:refractionSearchRequest, userId: xsd:string)
     ns0:searchRefractionsResponse(refraction: ns0:refraction[])
     ns0:searchSales(searchRequest: ns0:salesSearchRequest, userId: xsd:string)
     ns0:searchSalesResponse(salesList: ns0:salesItem[])
     ns0:searchScheduleItems(searchRequest: ns0:scheduleItemSearchRequest, userId: xsd:string)
     ns0:searchScheduleItemsResponse(scheduleItemList: ns0:scheduleItem[])
     ns0:searchServices(searchRequest: ns0:serviceSearchRequest, userId: xsd:string)
     ns0:searchServicesResponse(serviceList: ns0:serviceBasic[])
     ns0:searchTodaysInProgressEncounters(locationId: xsd:long, userId: xsd:string)
     ns0:searchTodaysInProgressEncountersResponse(encounterList: ns0:encounterBasic[])
     ns0:searchTransactions(searchRequest: ns0:transactionSearchRequest, userId: xsd:string)
     ns0:searchTransactionsResponse(transactionList: ns0:transactionWithPayor[])
     ns0:searchTransactionsV2(searchRequest: ns0:transactionExtendedSearchRequest, userId: xsd:string)
     ns0:searchTransactionsV2Response(transactionList: ns0:transactionWithPayor[])
     ns0:searchTransactionsWithDiagnoses(searchRequest: ns0:transactionSearchRequest, userId: xsd:string)
     ns0:searchTransactionsWithDiagnosesResponse(transactionList: ns0:transactionWithDiagnoses[])
     ns0:serviceBasic(active: xsd:boolean, additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, commonDescription: xsd:string, fullName: xsd:string, id: xsd:long, invoiceDescription: xsd:string, longDescription: xsd:string, name: xsd:string, price: xsd:double, serviceType: xsd:int, shortDescription: xsd:string, taxName: xsd:string, taxRate: xsd:double)   
     ns0:serviceSearchRequest(activeOnly: xsd:boolean, locationId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, updatedSince: xsd:string)
     ns0:setPatientNotified(orderNotificationStatusUpdateRequest: ns0:orderNotificationStatusUpdateRequest, userId: xsd:string)
     ns0:setPatientNotifiedResponse(updatedOrder: ns0:orderDetail)
     ns0:softContactLensRxInfo(addPower: xsd:double, axis: xsd:int, baseCurve: xsd:double, cylinder: xsd:double, diameter: xsd:double, lensColorCode: xsd:string, lensColorGenericName: xsd:string, lensColorName: xsd:string, monovision: xsd:boolean, product: ns0:productBasic, sphere: xsd:double, addDesignation: xsd:string)
     ns0:transaction(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, adjustment: xsd:double, balance: 
xsd:double, brandId: xsd:long, brandName: xsd:string, code: xsd:string, collectionId: xsd:long, collectionName: xsd:string, description: xsd:string, discountTotal: xsd:double, extendedPrice: xsd:double, id: xsd:long, invoiceApprovedDate: xsd:string, 
invoiceEmployeePersonId: xsd:long, invoiceId: xsd:long, invoiceStatus: xsd:int, itemEmployeePersonId: xsd:long, itemType: xsd:int, locationId: xsd:long, locationProductId: xsd:long, manufacturerId: xsd:long, manufacturerName: xsd:string, orderId: xsd:long, patientId: xsd:long, postDate: xsd:string, practiceId: xsd:long, productCategoryId: xsd:long, productCategoryName: xsd:string, productId: xsd:long, productUPC: xsd:string, providerCredentials: xsd:string, providerFirstName: xsd:string, providerId: xsd:long, providerLastName: xsd:string, quantity: xsd:int, serviceDate: xsd:string, serviceId: xsd:long, status: xsd:int, tax: xsd:double, totalPrice: xsd:double, unitPrice: xsd:double)
     ns0:transactionDiagnosis(codeSet: xsd:string, createdDate: xsd:string, diagnosisCode: xsd:string, diagnosisDate: xsd:string, encounterId: xsd:long, isMasterDiagnosis: xsd:boolean, isPrimary: xsd:boolean, location: xsd:string, patientDiagnosisId: xsd:long, qualifier: xsd:string, resolutionDate: xsd:string, status: xsd:string, updatedDate: xsd:string)
     ns0:transactionExtendedSearchRequest(endDate: xsd:string, invoiceStatuses: xsd:int[], itemStatuses: xsd:int[], itemTypes: xsd:int[], locationId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, productCategoryIds: xsd:long[], startDate: xsd:string, updatedSince: xsd:string, serviceEndDate: xsd:string, serviceStartDate: xsd:string)
     ns0:transactionSearchRequest(endDate: xsd:string, invoiceStatuses: xsd:int[], itemStatuses: xsd:int[], itemTypes: xsd:int[], locationId: xsd:long, pageNumber: xsd:int, pageSize: xsd:int, patientId: xsd:long, productCategoryIds: xsd:long[], startDate: xsd:string, updatedSince: xsd:string)
     ns0:transactionWithDiagnoses(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, adjustment: xsd:double, balance: xsd:double, brandId: xsd:long, brandName: xsd:string, code: xsd:string, collectionId: xsd:long, collectionName: 
xsd:string, description: xsd:string, discountTotal: xsd:double, extendedPrice: xsd:double, id: xsd:long, invoiceApprovedDate: xsd:string, invoiceEmployeePersonId: xsd:long, invoiceId: xsd:long, invoiceStatus: xsd:int, itemEmployeePersonId: xsd:long, 
itemType: xsd:int, locationId: xsd:long, locationProductId: xsd:long, manufacturerId: xsd:long, manufacturerName: xsd:string, orderId: xsd:long, patientId: xsd:long, postDate: xsd:string, practiceId: xsd:long, productCategoryId: xsd:long, productCategoryName: xsd:string, productId: xsd:long, productUPC: xsd:string, providerCredentials: xsd:string, providerFirstName: xsd:string, providerId: xsd:long, providerLastName: xsd:string, quantity: xsd:int, serviceDate: xsd:string, serviceId: xsd:long, status: xsd:int, tax: xsd:double, totalPrice: xsd:double, unitPrice: xsd:double, payor: ns0:payor, diagnoses: ns0:transactionDiagnosis[])
     ns0:transactionWithPayor(additionalProperties: {entry: {key: xsd:string, value: xsd:string}[]}, adjustment: xsd:double, 
balance: xsd:double, brandId: xsd:long, brandName: xsd:string, code: xsd:string, collectionId: xsd:long, collectionName: xsd:string, description: xsd:string, discountTotal: xsd:double, extendedPrice: xsd:double, id: xsd:long, invoiceApprovedDate: xsd:string, invoiceEmployeePersonId: xsd:long, invoiceId: xsd:long, invoiceStatus: xsd:int, itemEmployeePersonId: xsd:long, itemType: xsd:int, locationId: xsd:long, locationProductId: xsd:long, manufacturerId: xsd:long, manufacturerName: xsd:string, orderId: xsd:long, patientId: xsd:long, postDate: xsd:string, practiceId: xsd:long, productCategoryId: xsd:long, productCategoryName: xsd:string, productId: xsd:long, productUPC: xsd:string, providerCredentials: xsd:string, providerFirstName: xsd:string, providerId: xsd:long, providerLastName: xsd:string, quantity: xsd:int, serviceDate: xsd:string, serviceId: xsd:long, status: xsd:int, tax: xsd:double, totalPrice: xsd:double, unitPrice: xsd:double, payor: ns0:payor)
     ns0:updateOrderStatus(orderStatusUpdateRequest: ns0:orderStatusUpdateRequest, userId: xsd:string)
     ns0:updateOrderStatusResponse(result: xsd:string)
     ns0:updatePatient(patient: ns0:patientMinimal, userId: xsd:string)
     ns0:updatePatientCommunicationPreferences(patientId: xsd:long, commPreferences: ns0:patientCommunicationPreferenceUpdate[], userId: xsd:string)
     ns0:updatePatientCommunicationPreferencesResponse(result: xsd:string)
     ns0:updatePatientLogin(patientLogin: ns0:patientLogin, userId: xsd:string)
     ns0:updatePatientLoginResponse(result: xsd:string)
     ns0:updatePatientResponse(result: xsd:string)
     ns0:uploadPatientFilesToFolder(patientId: xsd:long, folderName: xsd:string, files: ns0:fileUpload[], userId: xsd:string)     ns0:uploadPatientFilesToFolderResponse(patientFileList: ns0:patientFile[])
     ns0:verifyPatientUserNameAvailable(userName: xsd:string, userId: xsd:string)
     ns0:verifyPatientUserNameAvailableResponse(available: xsd:boolean)
     xsd:ENTITIES
     xsd:ENTITY
     xsd:ID
     xsd:IDREF
     xsd:IDREFS
     xsd:NCName
     xsd:NMTOKEN
     xsd:NMTOKENS
     xsd:NOTATION
     xsd:Name
     xsd:QName
     xsd:anySimpleType
     xsd:anyURI
     xsd:base64Binary
     xsd:boolean
     xsd:byte
     xsd:date
     xsd:dateTime
     xsd:decimal
     xsd:double
     xsd:duration
     xsd:float
     xsd:gDay
     xsd:gMonth
     xsd:gMonthDay
     xsd:gYear
     xsd:gYearMonth
     xsd:hexBinary
     xsd:int
     xsd:integer
     xsd:language
     xsd:long
     xsd:negativeInteger
     xsd:nonNegativeInteger
     xsd:nonPositiveInteger
     xsd:normalizedString
     xsd:positiveInteger
     xsd:short
     xsd:string
     xsd:time
     xsd:token
     xsd:unsignedByte
     xsd:unsignedInt
     xsd:unsignedLong
     xsd:unsignedShort

Bindings:
     Soap12Binding: {http://ws.partner.revolutionehr.com}PartnerServiceSoapBinding

Service: PartnerService
     Port: PartnerPort (Soap12Binding: {http://ws.partner.revolutionehr.com}PartnerServiceSoapBinding)
         Operations:
            activatePatient(patientId: xsd:long, userId: xsd:string) -> patient: ns0:patientBasic
            addPatient(patient: ns0:patientMinimal, userId: xsd:string) -> newPatientId: xsd:long
            cancelAppointment(appointmentId: xsd:long, patientInitiated: xsd:boolean, emailPatient: xsd:boolean, reason: xsd:string, userId: xsd:string) -> result: xsd:string
            confirmAppointment(appointmentId: xsd:long, comment: xsd:string, userId: xsd:string) -> result: xsd:string       
            createAppointmentFromDetails(createAppointmentRequest: ns0:createAppointmentRequest, userId: xsd:string) -> apptId: xsd:long
            createAppointmentFromSlot(createAppointmentFromSlotRequest: ns0:createAppointmentFromSlotRequest, userId: xsd:string) -> apptId: xsd:long
            deactivatePatient(patientId: xsd:long, userId: xsd:string) -> patient: ns0:patientBasic
            deceasePatient(patientId: xsd:long, dateOfDeath: xsd:string, userId: xsd:string) -> patient: ns0:patientBasic    
            echo(echoRequest: xsd:string, userId: xsd:string) -> echoResponse: xsd:string
            getAccountSummaryWithInsurance(patientId: xsd:long, userId: xsd:string) -> result: ns0:patientInsuranceAccountSummary
            getAllEmployees(userId: xsd:string) -> employeeList: ns0:employee[]
            getAllProviders(userId: xsd:string) -> providerList: ns0:provider[]
            getAppointmentById(appointmentId: xsd:long, userId: xsd:string) -> appointment: ns0:appointmentBasic
            getAppointmentDetailById(appointmentId: xsd:long, userId: xsd:string) -> appointment: ns0:appointmentDetail      
            getApptTypes(userId: xsd:string) -> apptTypeList: ns0:appointmentType[]
            getEmployeeIdByProviderId(providerId: xsd:long, userId: xsd:string) -> employeeId: xsd:long
            getEmployeeOffices(employeeId: xsd:long, userId: xsd:string) -> officeList: ns0:office[]
            getEmployees(userId: xsd:string) -> employeeList: ns0:employee[]
            getEncounterById(encounterId: xsd:long, userId: xsd:string) -> encounterList: ns0:encounterBasic
            getInsuranceCompanies(userId: xsd:string) -> companyList: ns0:insuranceCompany[]
            getInvoiceNotes(invoiceId: xsd:long, userId: xsd:string) -> noteList: ns0:note[]
            getKeyDatesForPatient(patientId: xsd:long, userId: xsd:string) -> patient: ns0:keyDatesBasic
            getOffices(userId: xsd:string) -> officeList: ns0:office[]
            getOrderDetailById(orderId: xsd:long, userId: xsd:string) -> order: ns0:orderDetail
            getPatientById(patientId: xsd:long, userId: xsd:string) -> patient: ns0:patientBasic
            getPatientInsuranceInfo(patientId: xsd:long, userId: xsd:string) -> insuranceInfo: ns0:insurance[]
            getPatientInsurancePriorities(userId: xsd:string) -> insurancePriority: ns0:insurancePriority[]
            getPatientInsuranceTypes(userId: xsd:string) -> insuranceType: ns0:insuranceType[]
            getPatientPhotoContent(patientPhotoId: xsd:long, userId: xsd:string) -> return: xsd:base64Binary
            getPatientSchedulingPreferences(patientId: xsd:long, userId: xsd:string) -> patientSchedulingPreferences: ns0:patientSchedulingPreferences
            getProviderIdByEmployeeId(employeeId: xsd:long, userId: xsd:string) -> providerId: xsd:long
            getProviders(userId: xsd:string) -> providerList: ns0:provider[]
            getRecallById(recallId: xsd:long, userId: xsd:string) -> recall: ns0:recallBasic
            getServerTime(userId: xsd:string) -> currentServerTime: xsd:string
            readinessCheck() ->
            rescheduleAppointmentFromDetails(rescheduleAppointmentRequest: ns0:rescheduleAppointmentRequest, userId: xsd:string) -> apptId: xsd:long
            searchAppointmentSlots(searchRequest: ns0:appointmentSlotSearchRequest, userId: xsd:string) -> appointmentSlotList: ns0:appointmentSlot[]
            searchAppointments(searchRequest: ns0:appointmentSearchRequest, userId: xsd:string) -> appointmentList: ns0:appointmentBasic[]
            searchAppointmentsWithDetail(searchRequest: ns0:appointmentSearchRequest, userId: xsd:string) -> appointmentList: ns0:appointmentDetail[]
            searchClaims(searchRequest: ns0:claimSearchRequest, userId: xsd:string) -> claims: ns0:insuranceClaim[]
            searchContactLensPrescriptions(searchRequest: ns0:contactLensPrescriptionSearchRequest, userId: xsd:string) -> contactLensPrescriptionList: ns0:contactLensPrescription[]
            searchDeletedRecalls(searchRequest: ns0:RecallSearchRequest, userId: xsd:string) -> deletedRecallList: ns0:deletedRecall[]
            searchEncounters(searchRequest: ns0:encounterSearchRequest, userId: xsd:string) -> encounterList: ns0:encounterBasic[]
            searchExternalMedicationPrescriptions(searchRequest: ns0:prescriptionSearchRequest, userId: xsd:string) -> medicationPrescription: ns0:medicationPrescription[]
            searchEyeglassPrescriptions(searchRequest: ns0:prescriptionSearchRequest, userId: xsd:string) -> eyeglassPrescriptionList: ns0:eyeglassPrescription[]
            searchInvoicePayments(searchRequest: ns0:paymentSearchRequest, userId: xsd:string) -> paymentList: ns0:payment[] 
            searchKeyDates(searchRequest: ns0:keyDatesSearchRequest, userId: xsd:string) -> keyDateList: ns0:keyDatesBasic[] 
            searchKeyDatesDetail(searchRequest: ns0:keyDatesSearchRequest, userId: xsd:string) -> return: ns0:keyDatesDetail[]
            searchMedicationPrescriptions(searchRequest: ns0:prescriptionSearchRequest, userId: xsd:string) -> medicationPrescription: ns0:medicationPrescription[]
            searchOrderDetail(searchRequest: ns0:orderSearchRequest, userId: xsd:string) -> orderDetailList: ns0:orderDetail[]
            searchOrders(searchRequest: ns0:orderSearchRequest, userId: xsd:string) -> orderList: ns0:orderBasic[]
            searchPatientBalances(patientId: ns0:patientBalanceSearchRequest, userId: xsd:string) -> patientBalanceList: ns0:patientBalance[]
            searchPatientDiagnoses(searchRequest: ns0:patientDiagnosisSearchRequest, userId: xsd:string) -> patientDiagnosisList: ns0:patientDiagnosis[]
            searchPatientInsuranceInfo(searchRequest: ns0:PatientInsuranceSearchRequest, userId: xsd:string) -> insuranceInfo: ns0:patientInsurance[]
            searchPatientPhotos(searchRequest: ns0:patientPhotoSearchRequest, userId: xsd:string) -> patientPhoto: ns0:patientPhoto[]
            searchPatientTransactions(searchRequest: ns0:transactionSearchRequest, userId: xsd:string) -> transactionList: ns0:transaction[]
            searchPatients(searchRequest: ns0:patientSearchRequest, userId: xsd:string) -> patientList: ns0:patientBasic[]   
            searchPatientsLimited(searchRequest: ns0:limitedPatientSearchRequest, userId: xsd:string) -> patientList: ns0:patientBasic[]
            searchPatientsWithReferral(searchRequest: ns0:patientSearchRequest, userId: xsd:string) -> patientList: ns0:patientWithReferral[]
            searchPaymentItems(searchRequest: ns0:paymentExtendedSearchRequest, userId: xsd:string) -> paymentList: ns0:payment[]
            searchPaymentItemsWithLedgerPostings(searchRequest: ns0:paymentDatesExtendedSearchRequest, userId: xsd:string) -> paymentList: ns0:paymentWithLedgerPostings[]
            searchPayments(searchRequest: ns0:paymentExtendedSearchRequest, userId: xsd:string) -> paymentList: ns0:payment[]            searchPaymentsWithLedgerPostings(searchRequest: ns0:paymentDatesExtendedSearchRequest, userId: xsd:string) -> paymentList: ns0:paymentWithLedgerPostings[]
mentList: ns0:paymentWithLedgerPostings[]
            searchProducts(searchRequest: ns0:productSearchRequest, userId: xsd:string) -> productList: ns0:productBasic[]
            searchRecalls(searchRequest: ns0:RecallSearchRequest, userId: xsd:string) -> recallList: ns0:recallBasic[]
            searchRefractions(searchRequest: ns0:refractionSearchRequest, userId: xsd:string) -> refraction: ns0:refraction[]            searchSales(searchRequest: ns0:salesSearchRequest, userId: xsd:string) -> salesList: ns0:salesItem[]
            searchScheduleItems(searchRequest: ns0:scheduleItemSearchRequest, userId: xsd:string) -> scheduleItemList: ns0:scheduleItem[]
            searchServices(searchRequest: ns0:serviceSearchRequest, userId: xsd:string) -> serviceList: ns0:serviceBasic[]
            searchTodaysInProgressEncounters(locationId: xsd:long, userId: xsd:string) -> encounterList: ns0:encounterBasic[]            searchTransactions(searchRequest: ns0:transactionSearchRequest, userId: xsd:string) -> transactionList: ns0:transactionWithPayor[]
            searchTransactionsV2(searchRequest: ns0:transactionExtendedSearchRequest, userId: xsd:string) -> transactionList: ns0:transactionWithPayor[]
            searchTransactionsWithDiagnoses(searchRequest: ns0:transactionSearchRequest, userId: xsd:string) -> transactionList: ns0:transactionWithDiagnoses[]
            setPatientNotified(orderNotificationStatusUpdateRequest: ns0:orderNotificationStatusUpdateRequest, userId: xsd:string) -> updatedOrder: ns0:orderDetail
            updateOrderStatus(orderStatusUpdateRequest: ns0:orderStatusUpdateRequest, userId: xsd:string) -> result: xsd:string
            updatePatient(patient: ns0:patientMinimal, userId: xsd:string) -> result: xsd:string
            updatePatientCommunicationPreferences(patientId: xsd:long, commPreferences: ns0:patientCommunicationPreferenceUpdate[], userId: xsd:string) -> result: xsd:string    
            updatePatientLogin(patientLogin: ns0:patientLogin, userId: xsd:string) -> result: xsd:string
            uploadPatientFilesToFolder(patientId: xsd:long, folderName: xsd:string, files: ns0:fileUpload[], userId: xsd:string) -> patientFileList: ns0:patientFile[]
            verifyPatientUserNameAvailable(userName: xsd:string, userId: xsd:string) -> available: xsd:boolean
```
## WSDL XML
```xml
<wsdl:definitions xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:wsp="http://www.w3.org/ns/ws-policy" xmlns:wsdl="http://schemas.xmlsoap.org/wsdl/" xmlns:wsaw="http://www.w3.org/2006/05/addressing/wsdl" xmlns:wsam="http://www.w3.org/2007/05/addressing/metadata" xmlns:tns="http://ws.partner.revolutionehr.com" xmlns:soap12="http://schemas.xmlsoap.org/wsdl/soap12/" xmlns:ns1="http://schemas.xmlsoap.org/soap/http" name="PartnerService" targetNamespace="http://ws.partner.revolutionehr.com">
  <wsdl:types>
    <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:tns="http://ws.partner.revolutionehr.com" attributeFormDefault="unqualified" elementFormDefault="unqualified" targetNamespace="http://ws.partner.revolutionehr.com">
      <xs:element name="activatePatient" type="tns:activatePatient"/>
      <xs:element name="activatePatientResponse" type="tns:activatePatientResponse"/>
      <xs:element name="addPatient" type="tns:addPatient"/>
      <xs:element name="addPatientResponse" type="tns:addPatientResponse"/>
      <xs:element name="cancelAppointment" type="tns:cancelAppointment"/>
      <xs:element name="cancelAppointmentResponse" type="tns:cancelAppointmentResponse"/>
      <xs:element name="confirmAppointment" type="tns:confirmAppointment"/>
      <xs:element name="confirmAppointmentResponse" type="tns:confirmAppointmentResponse"/>
      <xs:element name="createAppointmentFromDetails" type="tns:createAppointmentFromDetails"/>
      <xs:element name="createAppointmentFromDetailsResponse" type="tns:createAppointmentFromDetailsResponse"/>
      <xs:element name="createAppointmentFromSlot" type="tns:createAppointmentFromSlot"/>
      <xs:element name="createAppointmentFromSlotResponse" type="tns:createAppointmentFromSlotResponse"/>
      <xs:element name="deactivatePatient" type="tns:deactivatePatient"/>
      <xs:element name="deactivatePatientResponse" type="tns:deactivatePatientResponse"/>
      <xs:element name="deceasePatient" type="tns:deceasePatient"/>
      <xs:element name="deceasePatientResponse" type="tns:deceasePatientResponse"/>
      <xs:element name="echo" type="tns:echo"/>
      <xs:element name="echoResponse" type="tns:echoResponse"/>
      <xs:element name="getAccountSummaryWithInsurance" type="tns:getAccountSummaryWithInsurance"/>
      <xs:element name="getAccountSummaryWithInsuranceResponse" type="tns:getAccountSummaryWithInsuranceResponse"/>
      <xs:element name="getAllEmployees" type="tns:getAllEmployees"/>
      <xs:element name="getAllEmployeesResponse" type="tns:getAllEmployeesResponse"/>
      <xs:element name="getAllProviders" type="tns:getAllProviders"/>
      <xs:element name="getAllProvidersResponse" type="tns:getAllProvidersResponse"/>
      <xs:element name="getAppointmentById" type="tns:getAppointmentById"/>
      <xs:element name="getAppointmentByIdResponse" type="tns:getAppointmentByIdResponse"/>
      <xs:element name="getAppointmentDetailById" type="tns:getAppointmentDetailById"/>
      <xs:element name="getAppointmentDetailByIdResponse" type="tns:getAppointmentDetailByIdResponse"/>
      <xs:element name="getApptTypes" type="tns:getApptTypes"/>
      <xs:element name="getApptTypesResponse" type="tns:getApptTypesResponse"/>
      <xs:element name="getEmployeeIdByProviderId" type="tns:getEmployeeIdByProviderId"/>
      <xs:element name="getEmployeeIdByProviderIdResponse" type="tns:getEmployeeIdByProviderIdResponse"/>
      <xs:element name="getEmployeeOffices" type="tns:getEmployeeOffices"/>
      <xs:element name="getEmployeeOfficesResponse" type="tns:getEmployeeOfficesResponse"/>
      <xs:element name="getEmployees" type="tns:getEmployees"/>
      <xs:element name="getEmployeesResponse" type="tns:getEmployeesResponse"/>
      <xs:element name="getEncounterById" type="tns:getEncounterById"/>
      <xs:element name="getEncounterByIdResponse" type="tns:getEncounterByIdResponse"/>
      <xs:element name="getInsuranceCompanies" type="tns:getInsuranceCompanies"/>
      <xs:element name="getInsuranceCompaniesResponse" type="tns:getInsuranceCompaniesResponse"/>
      <xs:element name="getInvoiceNotes" type="tns:getInvoiceNotes"/>
      <xs:element name="getInvoiceNotesResponse" type="tns:getInvoiceNotesResponse"/>
      <xs:element name="getKeyDatesForPatient" type="tns:getKeyDatesForPatient"/>
      <xs:element name="getKeyDatesForPatientResponse" type="tns:getKeyDatesForPatientResponse"/>
      <xs:element name="getOffices" type="tns:getOffices"/>
      <xs:element name="getOfficesResponse" type="tns:getOfficesResponse"/>
      <xs:element name="getOrderDetailById" type="tns:getOrderDetailById"/>
      <xs:element name="getOrderDetailByIdResponse" type="tns:getOrderDetailByIdResponse"/>
      <xs:element name="getPatientById" type="tns:getPatientById"/>
      <xs:element name="getPatientByIdResponse" type="tns:getPatientByIdResponse"/>
      <xs:element name="getPatientInsuranceInfo" type="tns:getPatientInsuranceInfo"/>
      <xs:element name="getPatientInsuranceInfoResponse" type="tns:getPatientInsuranceInfoResponse"/>
      <xs:element name="getPatientInsurancePriorities" type="tns:getPatientInsurancePriorities"/>
      <xs:element name="getPatientInsurancePrioritiesResponse" type="tns:getPatientInsurancePrioritiesResponse"/>
      <xs:element name="getPatientInsuranceTypes" type="tns:getPatientInsuranceTypes"/>
      <xs:element name="getPatientInsuranceTypesResponse" type="tns:getPatientInsuranceTypesResponse"/>
      <xs:element name="getPatientPhotoContent" type="tns:getPatientPhotoContent"/>
      <xs:element name="getPatientPhotoContentResponse" type="tns:getPatientPhotoContentResponse"/>
      <xs:element name="getPatientSchedulingPreferences" type="tns:getPatientSchedulingPreferences"/>
      <xs:element name="getPatientSchedulingPreferencesResponse" type="tns:getPatientSchedulingPreferencesResponse"/>
      <xs:element name="getProviderIdByEmployeeId" type="tns:getProviderIdByEmployeeId"/>
      <xs:element name="getProviderIdByEmployeeIdResponse" type="tns:getProviderIdByEmployeeIdResponse"/>
      <xs:element name="getProviders" type="tns:getProviders"/>
      <xs:element name="getProvidersResponse" type="tns:getProvidersResponse"/>
      <xs:element name="getRecallById" type="tns:getRecallById"/>
      <xs:element name="getRecallByIdResponse" type="tns:getRecallByIdResponse"/>
      <xs:element name="getServerTime" type="tns:getServerTime"/>
      <xs:element name="getServerTimeResponse" type="tns:getServerTimeResponse"/>
      <xs:element name="readinessCheck" type="tns:readinessCheck"/>
      <xs:element name="readinessCheckResponse" type="tns:readinessCheckResponse"/>
      <xs:element name="rescheduleAppointmentFromDetails" type="tns:rescheduleAppointmentFromDetails"/>
      <xs:element name="rescheduleAppointmentFromDetailsResponse" type="tns:rescheduleAppointmentFromDetailsResponse"/>
      <xs:element name="searchAppointmentSlots" type="tns:searchAppointmentSlots"/>
      <xs:element name="searchAppointmentSlotsResponse" type="tns:searchAppointmentSlotsResponse"/>
      <xs:element name="searchAppointments" type="tns:searchAppointments"/>
      <xs:element name="searchAppointmentsResponse" type="tns:searchAppointmentsResponse"/>
      <xs:element name="searchAppointmentsWithDetail" type="tns:searchAppointmentsWithDetail"/>
      <xs:element name="searchAppointmentsWithDetailResponse" type="tns:searchAppointmentsWithDetailResponse"/>
      <xs:element name="searchClaims" type="tns:searchClaims"/>
      <xs:element name="searchClaimsResponse" type="tns:searchClaimsResponse"/>
      <xs:element name="searchContactLensPrescriptions" type="tns:searchContactLensPrescriptions"/>
      <xs:element name="searchContactLensPrescriptionsResponse" type="tns:searchContactLensPrescriptionsResponse"/>
      <xs:element name="searchDeletedRecalls" type="tns:searchDeletedRecalls"/>
      <xs:element name="searchDeletedRecallsResponse" type="tns:searchDeletedRecallsResponse"/>
      <xs:element name="searchEncounters" type="tns:searchEncounters"/>
      <xs:element name="searchEncountersResponse" type="tns:searchEncountersResponse"/>
      <xs:element name="searchExternalMedicationPrescriptions" type="tns:searchExternalMedicationPrescriptions"/>
      <xs:element name="searchExternalMedicationPrescriptionsResponse" type="tns:searchExternalMedicationPrescriptionsResponse"/>
      <xs:element name="searchEyeglassPrescriptions" type="tns:searchEyeglassPrescriptions"/>
      <xs:element name="searchEyeglassPrescriptionsResponse" type="tns:searchEyeglassPrescriptionsResponse"/>
      <xs:element name="searchInvoicePayments" type="tns:searchInvoicePayments"/>
      <xs:element name="searchInvoicePaymentsResponse" type="tns:searchInvoicePaymentsResponse"/>
      <xs:element name="searchKeyDates" type="tns:searchKeyDates"/>
      <xs:element name="searchKeyDatesDetail" type="tns:searchKeyDatesDetail"/>
      <xs:element name="searchKeyDatesDetailResponse" type="tns:searchKeyDatesDetailResponse"/>
      <xs:element name="searchKeyDatesResponse" type="tns:searchKeyDatesResponse"/>
      <xs:element name="searchMedicationPrescriptions" type="tns:searchMedicationPrescriptions"/>
      <xs:element name="searchMedicationPrescriptionsResponse" type="tns:searchMedicationPrescriptionsResponse"/>
      <xs:element name="searchOrderDetail" type="tns:searchOrderDetail"/>
      <xs:element name="searchOrderDetailResponse" type="tns:searchOrderDetailResponse"/>
      <xs:element name="searchOrders" type="tns:searchOrders"/>
      <xs:element name="searchOrdersResponse" type="tns:searchOrdersResponse"/>
      <xs:element name="searchPatientBalances" type="tns:searchPatientBalances"/>
      <xs:element name="searchPatientBalancesResponse" type="tns:searchPatientBalancesResponse"/>
      <xs:element name="searchPatientDiagnoses" type="tns:searchPatientDiagnoses"/>
      <xs:element name="searchPatientDiagnosesResponse" type="tns:searchPatientDiagnosesResponse"/>
      <xs:element name="searchPatientInsuranceInfo" type="tns:searchPatientInsuranceInfo"/>
      <xs:element name="searchPatientInsuranceInfoResponse" type="tns:searchPatientInsuranceInfoResponse"/>
      <xs:element name="searchPatientPhotos" type="tns:searchPatientPhotos"/>
      <xs:element name="searchPatientPhotosResponse" type="tns:searchPatientPhotosResponse"/>
      <xs:element name="searchPatientTransactions" type="tns:searchPatientTransactions"/>
      <xs:element name="searchPatientTransactionsResponse" type="tns:searchPatientTransactionsResponse"/>
      <xs:element name="searchPatients" type="tns:searchPatients"/>
      <xs:element name="searchPatientsLimited" type="tns:searchPatientsLimited"/>
      <xs:element name="searchPatientsLimitedResponse" type="tns:searchPatientsLimitedResponse"/>
      <xs:element name="searchPatientsResponse" type="tns:searchPatientsResponse"/>
      <xs:element name="searchPatientsWithReferral" type="tns:searchPatientsWithReferral"/>
      <xs:element name="searchPatientsWithReferralResponse" type="tns:searchPatientsWithReferralResponse"/>
      <xs:element name="searchPaymentItems" type="tns:searchPaymentItems"/>
      <xs:element name="searchPaymentItemsResponse" type="tns:searchPaymentItemsResponse"/>
      <xs:element name="searchPaymentItemsWithLedgerPostings" type="tns:searchPaymentItemsWithLedgerPostings"/>
      <xs:element name="searchPaymentItemsWithLedgerPostingsResponse" type="tns:searchPaymentItemsWithLedgerPostingsResponse"/>
      <xs:element name="searchPayments" type="tns:searchPayments"/>
      <xs:element name="searchPaymentsResponse" type="tns:searchPaymentsResponse"/>
      <xs:element name="searchPaymentsWithLedgerPostings" type="tns:searchPaymentsWithLedgerPostings"/>
      <xs:element name="searchPaymentsWithLedgerPostingsResponse" type="tns:searchPaymentsWithLedgerPostingsResponse"/>
      <xs:element name="searchProducts" type="tns:searchProducts"/>
      <xs:element name="searchProductsResponse" type="tns:searchProductsResponse"/>
      <xs:element name="searchRecalls" type="tns:searchRecalls"/>
      <xs:element name="searchRecallsResponse" type="tns:searchRecallsResponse"/>
      <xs:element name="searchRefractions" type="tns:searchRefractions"/>
      <xs:element name="searchRefractionsResponse" type="tns:searchRefractionsResponse"/>
      <xs:element name="searchSales" type="tns:searchSales"/>
      <xs:element name="searchSalesResponse" type="tns:searchSalesResponse"/>
      <xs:element name="searchScheduleItems" type="tns:searchScheduleItems"/>
      <xs:element name="searchScheduleItemsResponse" type="tns:searchScheduleItemsResponse"/>
      <xs:element name="searchServices" type="tns:searchServices"/>
      <xs:element name="searchServicesResponse" type="tns:searchServicesResponse"/>
      <xs:element name="searchTodaysInProgressEncounters" type="tns:searchTodaysInProgressEncounters"/>
      <xs:element name="searchTodaysInProgressEncountersResponse" type="tns:searchTodaysInProgressEncountersResponse"/>
      <xs:element name="searchTransactions" type="tns:searchTransactions"/>
      <xs:element name="searchTransactionsResponse" type="tns:searchTransactionsResponse"/>
      <xs:element name="searchTransactionsV2" type="tns:searchTransactionsV2"/>
      <xs:element name="searchTransactionsV2Response" type="tns:searchTransactionsV2Response"/>
      <xs:element name="searchTransactionsWithDiagnoses" type="tns:searchTransactionsWithDiagnoses"/>
      <xs:element name="searchTransactionsWithDiagnosesResponse" type="tns:searchTransactionsWithDiagnosesResponse"/>
      <xs:element name="setPatientNotified" type="tns:setPatientNotified"/>
      <xs:element name="setPatientNotifiedResponse" type="tns:setPatientNotifiedResponse"/>
      <xs:element name="updateOrderStatus" type="tns:updateOrderStatus"/>
      <xs:element name="updateOrderStatusResponse" type="tns:updateOrderStatusResponse"/>
      <xs:element name="updatePatient" type="tns:updatePatient"/>
      <xs:element name="updatePatientCommunicationPreferences" type="tns:updatePatientCommunicationPreferences"/>
      <xs:element name="updatePatientCommunicationPreferencesResponse" type="tns:updatePatientCommunicationPreferencesResponse"/>
      <xs:element name="updatePatientLogin" type="tns:updatePatientLogin"/>
      <xs:element name="updatePatientLoginResponse" type="tns:updatePatientLoginResponse"/>
      <xs:element name="updatePatientResponse" type="tns:updatePatientResponse"/>
      <xs:element name="uploadPatientFilesToFolder" type="tns:uploadPatientFilesToFolder"/>
      <xs:element name="uploadPatientFilesToFolderResponse" type="tns:uploadPatientFilesToFolderResponse"/>
      <xs:element name="verifyPatientUserNameAvailable" type="tns:verifyPatientUserNameAvailable"/>
      <xs:element name="verifyPatientUserNameAvailableResponse" type="tns:verifyPatientUserNameAvailableResponse"/>
      <xs:complexType name="searchPaymentItems">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:paymentExtendedSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="paymentExtendedSearchRequest">
        <xs:complexContent>
          <xs:extension base="tns:paymentSearchRequest">
            <xs:sequence>
              <xs:element minOccurs="0" name="payorType" type="xs:int"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="paymentSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPaymentItemsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="paymentList" type="tns:payment"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="payment">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element name="amount" type="xs:double"/>
          <xs:element name="cardType" type="xs:int"/>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="invoiceItemId" type="xs:long"/>
          <xs:element minOccurs="0" name="paymentDate" type="xs:string"/>
          <xs:element minOccurs="0" name="paymentId" type="xs:long"/>
          <xs:element name="paymentMethod" type="xs:int"/>
          <xs:element minOccurs="0" name="payor" type="tns:payor"/>
          <xs:element minOccurs="0" name="referenceNumber" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="payor">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element minOccurs="0" name="payorId" type="xs:long"/>
          <xs:element name="type" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="deactivatePatient">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="deactivatePatientResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:patientBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientBasic">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="address" type="tns:address"/>
          <xs:element minOccurs="0" name="cellPhone" type="xs:string"/>
          <xs:element name="commApptMask" type="xs:int"/>
          <xs:element name="commApptOptIn" type="xs:int"/>
          <xs:element name="commGeneralMask" type="xs:int"/>
          <xs:element name="commGeneralOptIn" type="xs:int"/>
          <xs:element name="commOrderMask" type="xs:int"/>
          <xs:element name="commOrderOptIn" type="xs:int"/>
          <xs:element name="commRecallMask" type="xs:int"/>
          <xs:element name="commRecallOptIn" type="xs:int"/>
          <xs:element minOccurs="0" name="credentials" type="xs:string"/>
          <xs:element minOccurs="0" name="dob" type="xs:string"/>
          <xs:element minOccurs="0" name="email" type="xs:string"/>
          <xs:element minOccurs="0" name="familyAccountId" type="xs:long"/>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="gender" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorAddress" type="tns:address"/>
          <xs:element minOccurs="0" name="guarantorCellPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorCellPhoneExt" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorCredentials" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorEmail" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorHomePhone" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorHomePhoneExt" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorId" type="xs:long"/>
          <xs:element minOccurs="0" name="guarantorLastName" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorMiddleName" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorNickName" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorSuffix" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorWorkPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="guarantorWorkPhoneExt" type="xs:string"/>
          <xs:element minOccurs="0" name="headOfHousehold" type="xs:boolean"/>
          <xs:element minOccurs="0" name="homePhone" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element minOccurs="0" name="lastUpdated" type="xs:string"/>
          <xs:element minOccurs="0" name="maskedSsn" type="xs:string"/>
          <xs:element minOccurs="0" name="middleName" type="xs:string"/>
          <xs:element minOccurs="0" name="nickName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="preferredPhoneNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="primaryLocationId" type="xs:long"/>
          <xs:element minOccurs="0" name="primaryProviderId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="status" type="xs:string"/>
          <xs:element minOccurs="0" name="suffix" type="xs:string"/>
          <xs:element minOccurs="0" name="workPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="workPhoneExt" type="xs:string"/>
          <xs:element name="commOptOutMask" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="address">
        <xs:sequence>
          <xs:element minOccurs="0" name="address1" type="xs:string"/>
          <xs:element minOccurs="0" name="address2" type="xs:string"/>
          <xs:element minOccurs="0" name="city" type="xs:string"/>
          <xs:element minOccurs="0" name="country" type="xs:string"/>
          <xs:element minOccurs="0" name="postalCode" type="xs:string"/>
          <xs:element minOccurs="0" name="stateProvince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="uploadPatientFilesToFolder">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="folderName" type="xs:string"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="files" type="tns:fileUpload"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="fileUpload">
        <xs:sequence>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="data" type="xs:base64Binary"/>
          <xs:element minOccurs="0" name="fileName" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="uploadPatientFilesToFolderResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientFileList" type="tns:patientFile"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientFile">
        <xs:sequence>
          <xs:element minOccurs="0" name="file" type="tns:file"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="file">
        <xs:sequence>
          <xs:element minOccurs="0" name="contentType" type="xs:string"/>
          <xs:element minOccurs="0" name="createdOn" type="xs:string"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element minOccurs="0" name="fileName" type="xs:string"/>
          <xs:element name="fileSize" type="xs:long"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="mimeType" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedOn" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getInvoiceNotes">
        <xs:sequence>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getInvoiceNotesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="noteList" type="tns:note"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="note">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="categoryId" type="xs:long"/>
          <xs:element minOccurs="0" name="createdBy" type="xs:string"/>
          <xs:element minOccurs="0" name="createdOn" type="xs:string"/>
          <xs:element minOccurs="0" name="entityId" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="parentId" type="xs:long"/>
          <xs:element minOccurs="0" name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="subCategoryId" type="xs:long"/>
          <xs:element minOccurs="0" name="text" type="xs:string"/>
          <xs:element minOccurs="0" name="user" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getRecallById">
        <xs:sequence>
          <xs:element minOccurs="0" name="recallId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getRecallByIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="recall" type="tns:recallBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="recallBasic">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="lastUpdated" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="recallComments" type="xs:string"/>
          <xs:element minOccurs="0" name="recallDate" type="xs:string"/>
          <xs:element minOccurs="0" name="recallId" type="xs:long"/>
          <xs:element minOccurs="0" name="recallReason" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="setPatientNotified">
        <xs:sequence>
          <xs:element minOccurs="0" name="orderNotificationStatusUpdateRequest" type="tns:orderNotificationStatusUpdateRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderNotificationStatusUpdateRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="notificationComments" type="xs:string"/>
          <xs:element minOccurs="0" name="notifiedDate" type="xs:string"/>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="setPatientNotifiedResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="updatedOrder" type="tns:orderDetail"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetail">
        <xs:complexContent>
          <xs:extension base="tns:orderBasic">
            <xs:sequence/>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="orderBasic">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="createdOn" type="xs:string"/>
          <xs:element minOccurs="0" name="instructions" type="xs:string"/>
          <xs:element minOccurs="0" name="lastUpdated" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
          <xs:element name="orderType" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element name="patientNotified" type="xs:boolean"/>
          <xs:element name="shipToType" type="xs:int"/>
          <xs:element name="statusCode" type="xs:int"/>
          <xs:element minOccurs="0" name="statusDate" type="xs:string"/>
          <xs:element minOccurs="0" name="statusName" type="xs:string"/>
          <xs:element minOccurs="0" name="vendorName" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailEyeglasses">
        <xs:complexContent>
          <xs:extension base="tns:orderDetail">
            <xs:sequence>
              <xs:element minOccurs="0" name="binocularPdDistance" type="xs:double"/>
              <xs:element minOccurs="0" name="binocularPdNear" type="xs:double"/>
              <xs:element minOccurs="0" name="frameIndication" type="xs:int"/>
              <xs:element minOccurs="0" name="frameInfo" type="tns:orderDetailFrameInfo"/>
              <xs:element minOccurs="0" name="frameProduct" type="tns:productBasic"/>
              <xs:element minOccurs="0" name="lensRequest" type="xs:int"/>
              <xs:element minOccurs="0" name="odLens" type="tns:orderDetailLens"/>
              <xs:element maxOccurs="unbounded" minOccurs="0" name="options" nillable="true" type="tns:orderDetailOption"/>
              <xs:element minOccurs="0" name="osLens" type="tns:orderDetailLens"/>
              <xs:element minOccurs="0" name="panto" type="xs:double"/>
              <xs:element minOccurs="0" name="polishEdges" type="xs:boolean"/>
              <xs:element minOccurs="0" name="prescription" type="tns:orderDetailEyeglassesRx"/>
              <xs:element minOccurs="0" name="quantity" type="xs:int"/>
              <xs:element minOccurs="0" name="rollEdges" type="xs:boolean"/>
              <xs:element minOccurs="0" name="wrapAngle" type="xs:double"/>
              <xs:element minOccurs="0" name="odLensProduct" type="tns:productBasic"/>
              <xs:element minOccurs="0" name="osLensProduct" type="tns:productBasic"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="orderDetailFrameInfo">
        <xs:sequence>
          <xs:element minOccurs="0" name="a" type="xs:double"/>
          <xs:element minOccurs="0" name="b" type="xs:double"/>
          <xs:element minOccurs="0" name="bridge" type="xs:double"/>
          <xs:element minOccurs="0" name="circumference" type="xs:double"/>
          <xs:element minOccurs="0" name="colorCode" type="xs:string"/>
          <xs:element minOccurs="0" name="colorName" type="xs:string"/>
          <xs:element minOccurs="0" name="dbl" type="xs:double"/>
          <xs:element minOccurs="0" name="ed" type="xs:double"/>
          <xs:element minOccurs="0" name="edAngle" type="xs:double"/>
          <xs:element minOccurs="0" name="eye" type="xs:double"/>
          <xs:element minOccurs="0" name="genericColorName" type="xs:string"/>
          <xs:element minOccurs="0" name="lensColorCode" type="xs:string"/>
          <xs:element minOccurs="0" name="lensColorName" type="xs:string"/>
          <xs:element minOccurs="0" name="screwToScrew" type="xs:double"/>
          <xs:element minOccurs="0" name="temple" type="xs:double"/>
          <xs:element minOccurs="0" name="templeUnit" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="productBasic">
        <xs:sequence>
          <xs:element name="active" type="xs:boolean"/>
          <xs:element name="actualCost" type="xs:double"/>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="brandId" type="xs:long"/>
          <xs:element minOccurs="0" name="brandName" type="xs:string"/>
          <xs:element minOccurs="0" name="categoryId" type="xs:long"/>
          <xs:element minOccurs="0" name="categoryName" type="xs:string"/>
          <xs:element minOccurs="0" name="collectionId" type="xs:long"/>
          <xs:element minOccurs="0" name="collectionName" type="xs:string"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element name="discontinued" type="xs:boolean"/>
          <xs:element minOccurs="0" name="locationProductId" type="xs:long"/>
          <xs:element minOccurs="0" name="manufacturerId" type="xs:long"/>
          <xs:element minOccurs="0" name="manufacturerName" type="xs:string"/>
          <xs:element name="master" type="xs:boolean"/>
          <xs:element name="multiplier" type="xs:double"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element minOccurs="0" name="productCode" type="xs:string"/>
          <xs:element minOccurs="0" name="productId" type="xs:long"/>
          <xs:element name="retailPrice" type="xs:double"/>
          <xs:element minOccurs="0" name="sku" type="xs:string"/>
          <xs:element minOccurs="0" name="upc" type="xs:string"/>
          <xs:element name="wholesalePrice" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailLens">
        <xs:sequence>
          <xs:element minOccurs="0" name="backVertexDistance" type="xs:double"/>
          <xs:element minOccurs="0" name="baseCurve" type="xs:double"/>
          <xs:element minOccurs="0" name="blankSize" type="xs:double"/>
          <xs:element minOccurs="0" name="monocularPd" type="xs:double"/>
          <xs:element minOccurs="0" name="monocularPdNear" type="xs:double"/>
          <xs:element minOccurs="0" name="opticalCenter" type="xs:double"/>
          <xs:element minOccurs="0" name="opticalCenterType" type="xs:int"/>
          <xs:element minOccurs="0" name="segHeight" type="xs:double"/>
          <xs:element minOccurs="0" name="segHeightType" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailOption">
        <xs:sequence>
          <xs:element minOccurs="0" name="categoryId" type="xs:int"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element minOccurs="0" name="product" type="tns:productBasic"/>
          <xs:element minOccurs="0" name="value" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailEyeglassesRx">
        <xs:sequence>
          <xs:element minOccurs="0" name="binocularPdDistance" type="xs:double"/>
          <xs:element minOccurs="0" name="binocularPdNear" type="xs:double"/>
          <xs:element minOccurs="0" name="odLensRx" type="tns:orderDetailLensRx"/>
          <xs:element minOccurs="0" name="osLensRx" type="tns:orderDetailLensRx"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailLensRx">
        <xs:sequence>
          <xs:element minOccurs="0" name="axis" type="xs:int"/>
          <xs:element minOccurs="0" name="balanced" type="xs:boolean"/>
          <xs:element minOccurs="0" name="cylinder" type="xs:double"/>
          <xs:element minOccurs="0" name="horizontalPrism" type="xs:double"/>
          <xs:element minOccurs="0" name="horizontalPrismOrientation" type="xs:string"/>
          <xs:element minOccurs="0" name="intermediateAdd" type="xs:double"/>
          <xs:element minOccurs="0" name="nearAdd" type="xs:double"/>
          <xs:element minOccurs="0" name="sphere" type="xs:double"/>
          <xs:element minOccurs="0" name="verticalPrism" type="xs:double"/>
          <xs:element minOccurs="0" name="verticalPrismOrientation" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailFrame">
        <xs:complexContent>
          <xs:extension base="tns:orderDetail">
            <xs:sequence>
              <xs:element minOccurs="0" name="frameInfo" type="tns:orderDetailFrameInfo"/>
              <xs:element minOccurs="0" name="product" type="tns:productBasic"/>
              <xs:element minOccurs="0" name="quantity" type="xs:int"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="orderDetailContactLens">
        <xs:complexContent>
          <xs:extension base="tns:orderDetail">
            <xs:sequence>
              <xs:element minOccurs="0" name="lensType" type="xs:int"/>
              <xs:element minOccurs="0" name="odLensRx" type="tns:orderDetailContactLensRx"/>
              <xs:element minOccurs="0" name="osLensRx" type="tns:orderDetailContactLensRx"/>
              <xs:element minOccurs="0" name="quantityOd" type="xs:int"/>
              <xs:element minOccurs="0" name="quantityOs" type="xs:int"/>
              <xs:element minOccurs="0" name="unitOd" type="xs:string"/>
              <xs:element minOccurs="0" name="unitOs" type="xs:string"/>
              <xs:element minOccurs="0" name="prescription" type="tns:prescription"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="orderDetailContactLensRx">
        <xs:sequence>
          <xs:element minOccurs="0" name="addPower" type="xs:double"/>
          <xs:element minOccurs="0" name="axis" type="xs:int"/>
          <xs:element minOccurs="0" name="baseCurve" type="xs:double"/>
          <xs:element minOccurs="0" name="cylinder" type="xs:double"/>
          <xs:element minOccurs="0" name="diameter" type="xs:double"/>
          <xs:element minOccurs="0" name="isMonovision" type="xs:boolean"/>
          <xs:element minOccurs="0" name="lensColorCode" type="xs:string"/>
          <xs:element minOccurs="0" name="lensColorGenericName" type="xs:string"/>
          <xs:element minOccurs="0" name="lensColorName" type="xs:string"/>
          <xs:element minOccurs="0" name="product" type="tns:productBasic"/>
          <xs:element minOccurs="0" name="sphere" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderDetailSoftContactLensRx">
        <xs:complexContent>
          <xs:extension base="tns:orderDetailContactLensRx">
            <xs:sequence>
              <xs:element minOccurs="0" name="addDesignation" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="orderDetailRigidContactLensRx">
        <xs:complexContent>
          <xs:extension base="tns:orderDetailContactLensRx">
            <xs:sequence>
              <xs:element minOccurs="0" name="addDiameter" type="xs:double"/>
              <xs:element minOccurs="0" name="backOpticalDiameter" type="xs:double"/>
              <xs:element minOccurs="0" name="baseCurve2" type="xs:double"/>
              <xs:element minOccurs="0" name="bcUnit" type="xs:string"/>
              <xs:element minOccurs="0" name="centerThickness" type="xs:double"/>
              <xs:element minOccurs="0" name="distanceZone" type="xs:double"/>
              <xs:element minOccurs="0" name="dot" type="xs:boolean"/>
              <xs:element minOccurs="0" name="edgeLift" type="xs:string"/>
              <xs:element minOccurs="0" name="edgeLiftAmount" type="xs:double"/>
              <xs:element minOccurs="0" name="fenestration" type="xs:boolean"/>
              <xs:element minOccurs="0" name="firstCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="firstCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="fourthCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="fourthCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="intermediateSegment" type="xs:double"/>
              <xs:element minOccurs="0" name="landingZoneAngle" type="xs:int"/>
              <xs:element minOccurs="0" name="lensMaterial" type="xs:string"/>
              <xs:element minOccurs="0" name="midPeripheralLimbalClearance" type="xs:string"/>
              <xs:element minOccurs="0" name="notes" type="xs:string"/>
              <xs:element minOccurs="0" name="opticZone" type="xs:double"/>
              <xs:element minOccurs="0" name="peripheralCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="peripheralCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="peripheralEdge" type="xs:string"/>
              <xs:element minOccurs="0" name="plasmaTreatment" type="xs:boolean"/>
              <xs:element minOccurs="0" name="profile" type="xs:string"/>
              <xs:element minOccurs="0" name="returnZoneDiameter" type="xs:int"/>
              <xs:element minOccurs="0" name="sagittalDepth" type="xs:double"/>
              <xs:element minOccurs="0" name="secondCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="secondCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="secondaryCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="secondaryCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="segmentHeight" type="xs:double"/>
              <xs:element minOccurs="0" name="specialCharacteristics" type="xs:string"/>
              <xs:element minOccurs="0" name="sphere2" type="xs:double"/>
              <xs:element minOccurs="0" name="thirdCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="thirdCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="truncation" type="xs:double"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="orderDetailHybridContactLensRx">
        <xs:complexContent>
          <xs:extension base="tns:orderDetailContactLensRx">
            <xs:sequence>
              <xs:element minOccurs="0" name="addZoneSize" type="xs:string"/>
              <xs:element minOccurs="0" name="design" type="xs:string"/>
              <xs:element minOccurs="0" name="segmentSize" type="xs:string"/>
              <xs:element minOccurs="0" name="skirtCurveRadius" type="xs:string"/>
              <xs:element minOccurs="0" name="vault" type="xs:int"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="prescription">
        <xs:sequence>
          <xs:element minOccurs="0" name="authorizationDate" type="xs:dateTime"/>
          <xs:element name="authorizationType" type="xs:int"/>
          <xs:element minOccurs="0" name="bodyLocationName" type="xs:string"/>
          <xs:element minOccurs="0" name="createdByUserName" type="xs:string"/>
          <xs:element minOccurs="0" name="createdOn" type="xs:dateTime"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element minOccurs="0" name="expirationDate" type="xs:dateTime"/>
          <xs:element minOccurs="0" name="externalSystemId" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="instructions" type="xs:string"/>
          <xs:element name="numRefillsAllowed" type="xs:int"/>
          <xs:element name="numRefillsRemaining" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="personId" type="xs:long"/>
          <xs:element minOccurs="0" name="phrEnabled" type="xs:boolean"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="reason" type="xs:string"/>
          <xs:element minOccurs="0" name="startDate" type="xs:dateTime"/>
          <xs:element name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="stopDate" type="xs:dateTime"/>
          <xs:element minOccurs="0" name="stopReasonId" type="xs:long"/>
          <xs:element minOccurs="0" name="updatedByUserName" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedOn" type="xs:dateTime"/>
          <xs:element minOccurs="0" name="useProviderSignature" type="xs:boolean"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="eyeglassPrescription">
        <xs:complexContent>
          <xs:extension base="tns:prescription">
            <xs:sequence>
              <xs:element name="arCoating" type="xs:boolean"/>
              <xs:element minOccurs="0" name="arCoatingComment" type="xs:string"/>
              <xs:element minOccurs="0" name="distancePd" type="xs:string"/>
              <xs:element minOccurs="0" name="lensType" type="xs:string"/>
              <xs:element minOccurs="0" name="lensTypeComment" type="xs:string"/>
              <xs:element minOccurs="0" name="lensTypeId" type="xs:long"/>
              <xs:element minOccurs="0" name="material" type="xs:string"/>
              <xs:element minOccurs="0" name="materialComment" type="xs:string"/>
              <xs:element minOccurs="0" name="materialId" type="xs:long"/>
              <xs:element minOccurs="0" name="nearPd" type="xs:string"/>
              <xs:element minOccurs="0" name="odAxis" type="xs:string"/>
              <xs:element minOccurs="0" name="odBalanced" type="xs:boolean"/>
              <xs:element minOccurs="0" name="odCylinder" type="xs:string"/>
              <xs:element minOccurs="0" name="odHorizontalPrism" type="xs:string"/>
              <xs:element minOccurs="0" name="odHorizontalPrismOrientation" type="xs:string"/>
              <xs:element minOccurs="0" name="odIntermediateAdd" type="xs:string"/>
              <xs:element minOccurs="0" name="odNearAdd" type="xs:string"/>
              <xs:element minOccurs="0" name="odSphere" type="xs:string"/>
              <xs:element minOccurs="0" name="odVerticalPrism" type="xs:string"/>
              <xs:element minOccurs="0" name="odVerticalPrismOrientation" type="xs:string"/>
              <xs:element minOccurs="0" name="osAxis" type="xs:string"/>
              <xs:element minOccurs="0" name="osBalanced" type="xs:boolean"/>
              <xs:element minOccurs="0" name="osCylinder" type="xs:string"/>
              <xs:element minOccurs="0" name="osHorizontalPrism" type="xs:string"/>
              <xs:element minOccurs="0" name="osHorizontalPrismOrientation" type="xs:string"/>
              <xs:element minOccurs="0" name="osIntermediateAdd" type="xs:string"/>
              <xs:element minOccurs="0" name="osNearAdd" type="xs:string"/>
              <xs:element minOccurs="0" name="osSphere" type="xs:string"/>
              <xs:element minOccurs="0" name="osVerticalPrism" type="xs:string"/>
              <xs:element minOccurs="0" name="osVerticalPrismOrientation" type="xs:string"/>
              <xs:element name="photochromic" type="xs:boolean"/>
              <xs:element minOccurs="0" name="photochromicComment" type="xs:string"/>
              <xs:element name="polarized" type="xs:boolean"/>
              <xs:element minOccurs="0" name="polarizedComment" type="xs:string"/>
              <xs:element minOccurs="0" name="tint" type="xs:string"/>
              <xs:element minOccurs="0" name="tintComment" type="xs:string"/>
              <xs:element minOccurs="0" name="tintId" type="xs:long"/>
              <xs:element minOccurs="0" name="usedForReason" type="xs:string"/>
              <xs:element minOccurs="0" name="usedForReasonId" type="xs:long"/>
              <xs:element name="uvTreatment" type="xs:boolean"/>
              <xs:element minOccurs="0" name="uvTreatmentComment" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="medicationPrescription">
        <xs:complexContent>
          <xs:extension base="tns:prescription">
            <xs:sequence>
              <xs:element name="dosageAmount" type="xs:double"/>
              <xs:element minOccurs="0" name="dosageUnit" type="xs:string"/>
              <xs:element minOccurs="0" name="drugBrandName" type="xs:string"/>
              <xs:element minOccurs="0" name="drugCode" type="xs:string"/>
              <xs:element name="drugCodeSet" type="xs:int"/>
              <xs:element minOccurs="0" name="drugDescription" type="xs:string"/>
              <xs:element minOccurs="0" name="drugGenericName" type="xs:string"/>
              <xs:element minOccurs="0" name="frequency" type="xs:string"/>
              <xs:element minOccurs="0" name="route" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="externalMedicationPrescription">
        <xs:complexContent>
          <xs:extension base="tns:medicationPrescription">
            <xs:sequence/>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="contactLensPrescription">
        <xs:complexContent>
          <xs:extension base="tns:prescription">
            <xs:sequence>
              <xs:element minOccurs="0" name="od" type="tns:contactLensRxInfo"/>
              <xs:element minOccurs="0" name="os" type="tns:contactLensRxInfo"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="contactLensRxInfo">
        <xs:sequence>
          <xs:element minOccurs="0" name="addPower" type="xs:double"/>
          <xs:element minOccurs="0" name="axis" type="xs:int"/>
          <xs:element minOccurs="0" name="baseCurve" type="xs:double"/>
          <xs:element minOccurs="0" name="cylinder" type="xs:double"/>
          <xs:element minOccurs="0" name="diameter" type="xs:double"/>
          <xs:element minOccurs="0" name="lensColorCode" type="xs:string"/>
          <xs:element minOccurs="0" name="lensColorGenericName" type="xs:string"/>
          <xs:element minOccurs="0" name="lensColorName" type="xs:string"/>
          <xs:element minOccurs="0" name="monovision" type="xs:boolean"/>
          <xs:element minOccurs="0" name="product" type="tns:productBasic"/>
          <xs:element minOccurs="0" name="sphere" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="softContactLensRxInfo">
        <xs:complexContent>
          <xs:extension base="tns:contactLensRxInfo">
            <xs:sequence>
              <xs:element minOccurs="0" name="addDesignation" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="rigidContactLensRxInfo">
        <xs:complexContent>
          <xs:extension base="tns:contactLensRxInfo">
            <xs:sequence>
              <xs:element minOccurs="0" name="addDiameter" type="xs:double"/>
              <xs:element minOccurs="0" name="backOpticalDiameter" type="xs:double"/>
              <xs:element minOccurs="0" name="baseCurve2" type="xs:double"/>
              <xs:element minOccurs="0" name="bcUnit" type="xs:string"/>
              <xs:element minOccurs="0" name="centerThickness" type="xs:double"/>
              <xs:element minOccurs="0" name="distanceZone" type="xs:double"/>
              <xs:element minOccurs="0" name="dot" type="xs:boolean"/>
              <xs:element minOccurs="0" name="edgeLift" type="xs:string"/>
              <xs:element minOccurs="0" name="edgeLiftAmount" type="xs:double"/>
              <xs:element minOccurs="0" name="fenestration" type="xs:boolean"/>
              <xs:element minOccurs="0" name="firstCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="firstCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="fourthCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="fourthCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="intermediateSegment" type="xs:double"/>
              <xs:element minOccurs="0" name="landingZoneAngle" type="xs:int"/>
              <xs:element minOccurs="0" name="lensMaterial" type="xs:string"/>
              <xs:element minOccurs="0" name="midPeripheralLimbalClearance" type="xs:string"/>
              <xs:element minOccurs="0" name="notes" type="xs:string"/>
              <xs:element minOccurs="0" name="opticZone" type="xs:double"/>
              <xs:element minOccurs="0" name="peripheralCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="peripheralCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="peripheralEdge" type="xs:string"/>
              <xs:element minOccurs="0" name="plasmaTreatment" type="xs:boolean"/>
              <xs:element minOccurs="0" name="profile" type="xs:string"/>
              <xs:element minOccurs="0" name="returnZoneDiameter" type="xs:int"/>
              <xs:element minOccurs="0" name="sagittalDepth" type="xs:double"/>
              <xs:element minOccurs="0" name="secondCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="secondCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="secondaryCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="secondaryCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="segmentHeight" type="xs:double"/>
              <xs:element minOccurs="0" name="specialCharacteristics" type="xs:string"/>
              <xs:element minOccurs="0" name="sphere2" type="xs:double"/>
              <xs:element minOccurs="0" name="thirdCurveRadius" type="xs:double"/>
              <xs:element minOccurs="0" name="thirdCurveWidth" type="xs:double"/>
              <xs:element minOccurs="0" name="truncation" type="xs:double"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="hybridContactLensRxInfo">
        <xs:complexContent>
          <xs:extension base="tns:contactLensRxInfo">
            <xs:sequence>
              <xs:element minOccurs="0" name="addZoneSize" type="xs:string"/>
              <xs:element minOccurs="0" name="design" type="xs:string"/>
              <xs:element minOccurs="0" name="segmentSize" type="xs:string"/>
              <xs:element minOccurs="0" name="skirtCurveRadius" type="xs:string"/>
              <xs:element minOccurs="0" name="vault" type="xs:int"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="searchContactLensPrescriptions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:contactLensPrescriptionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="contactLensPrescriptionSearchRequest">
        <xs:complexContent>
          <xs:extension base="tns:prescriptionSearchRequest">
            <xs:sequence>
              <xs:element maxOccurs="unbounded" minOccurs="0" name="contactLensTypeIds" nillable="true" type="xs:int"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="prescriptionSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="authorizationType" type="xs:int"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="expirationEndDate" type="xs:string"/>
          <xs:element minOccurs="0" name="expirationStartDate" type="xs:string"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchContactLensPrescriptionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="contactLensPrescriptionList" type="tns:contactLensPrescription"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="activatePatient">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="activatePatientResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:patientBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updatePatient">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:patientMinimal"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientMinimal">
        <xs:sequence>
          <xs:element minOccurs="0" name="address" type="tns:address"/>
          <xs:element minOccurs="0" name="cellPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="credentials" type="xs:string"/>
          <xs:element minOccurs="0" name="dob" type="xs:string"/>
          <xs:element minOccurs="0" name="email" type="xs:string"/>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="gender" type="xs:string"/>
          <xs:element minOccurs="0" name="homePhone" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element minOccurs="0" name="middleName" type="xs:string"/>
          <xs:element minOccurs="0" name="nickName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="preferredPhoneNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="primaryLocationId" type="xs:long"/>
          <xs:element minOccurs="0" name="primaryProviderId" type="xs:long"/>
          <xs:element minOccurs="0" name="suffix" type="xs:string"/>
          <xs:element minOccurs="0" name="workPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="workPhoneExt" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updatePatientResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientDiagnoses">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:patientDiagnosisSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientDiagnosisSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="codeSet" type="xs:string"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="diagnosisCodes" nillable="true" type="xs:string"/>
          <xs:element minOccurs="0" name="diagnosisDateEnd" type="xs:string"/>
          <xs:element minOccurs="0" name="diagnosisDateStart" type="xs:string"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="resolutionDateEnd" type="xs:string"/>
          <xs:element minOccurs="0" name="resolutionDateStart" type="xs:string"/>
          <xs:element name="searchMaster" type="xs:boolean"/>
          <xs:element minOccurs="0" name="status" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSinceDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientDiagnosesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientDiagnosisList" type="tns:patientDiagnosis"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientDiagnosis">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="assessedDate" type="xs:string"/>
          <xs:element minOccurs="0" name="codeSet" type="xs:string"/>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="createdDate" type="xs:string"/>
          <xs:element minOccurs="0" name="diagnosisCode" type="xs:string"/>
          <xs:element minOccurs="0" name="diagnosisDate" type="xs:string"/>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element name="isMasterDiagnosis" type="xs:boolean"/>
          <xs:element name="isPrimary" type="xs:boolean"/>
          <xs:element minOccurs="0" name="location" type="xs:string"/>
          <xs:element minOccurs="0" name="longDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="patientDiagnosisId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="personId" type="xs:long"/>
          <xs:element minOccurs="0" name="qualifier" type="xs:string"/>
          <xs:element minOccurs="0" name="reason" type="xs:string"/>
          <xs:element minOccurs="0" name="resolutionDate" type="xs:string"/>
          <xs:element minOccurs="0" name="shortDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="status" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientTransactions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:transactionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="transactionSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="invoiceStatuses" nillable="true" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="itemStatuses" nillable="true" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="itemTypes" nillable="true" type="xs:int"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="productCategoryIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientTransactionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="transactionList" type="tns:transaction"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="transaction">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element name="adjustment" type="xs:double"/>
          <xs:element name="balance" type="xs:double"/>
          <xs:element minOccurs="0" name="brandId" type="xs:long"/>
          <xs:element minOccurs="0" name="brandName" type="xs:string"/>
          <xs:element minOccurs="0" name="code" type="xs:string"/>
          <xs:element minOccurs="0" name="collectionId" type="xs:long"/>
          <xs:element minOccurs="0" name="collectionName" type="xs:string"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element name="discountTotal" type="xs:double"/>
          <xs:element name="extendedPrice" type="xs:double"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="invoiceApprovedDate" type="xs:string"/>
          <xs:element minOccurs="0" name="invoiceEmployeePersonId" type="xs:long"/>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element name="invoiceStatus" type="xs:int"/>
          <xs:element minOccurs="0" name="itemEmployeePersonId" type="xs:long"/>
          <xs:element name="itemType" type="xs:int"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="locationProductId" type="xs:long"/>
          <xs:element minOccurs="0" name="manufacturerId" type="xs:long"/>
          <xs:element minOccurs="0" name="manufacturerName" type="xs:string"/>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="postDate" type="xs:string"/>
          <xs:element minOccurs="0" name="practiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="productCategoryId" type="xs:long"/>
          <xs:element minOccurs="0" name="productCategoryName" type="xs:string"/>
          <xs:element minOccurs="0" name="productId" type="xs:long"/>
          <xs:element minOccurs="0" name="productUPC" type="xs:string"/>
          <xs:element minOccurs="0" name="providerCredentials" type="xs:string"/>
          <xs:element minOccurs="0" name="providerFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="providerLastName" type="xs:string"/>
          <xs:element name="quantity" type="xs:int"/>
          <xs:element minOccurs="0" name="serviceDate" type="xs:string"/>
          <xs:element minOccurs="0" name="serviceId" type="xs:long"/>
          <xs:element name="status" type="xs:int"/>
          <xs:element name="tax" type="xs:double"/>
          <xs:element name="totalPrice" type="xs:double"/>
          <xs:element name="unitPrice" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchDeletedRecalls">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:RecallSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="RecallSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchDeletedRecallsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="deletedRecallList" type="tns:deletedRecall"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="deletedRecall">
        <xs:sequence>
          <xs:element minOccurs="0" name="deletedOn" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="recallId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchTransactions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:transactionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchTransactionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="transactionList" type="tns:transactionWithPayor"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="transactionWithPayor">
        <xs:complexContent>
          <xs:extension base="tns:transaction">
            <xs:sequence>
              <xs:element minOccurs="0" name="payor" type="tns:payor"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="searchTransactionsWithDiagnoses">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:transactionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchTransactionsWithDiagnosesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="transactionList" type="tns:transactionWithDiagnoses"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="transactionWithDiagnoses">
        <xs:complexContent>
          <xs:extension base="tns:transactionWithPayor">
            <xs:sequence>
              <xs:element maxOccurs="unbounded" minOccurs="0" name="diagnoses" nillable="true" type="tns:transactionDiagnosis"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="transactionDiagnosis">
        <xs:sequence>
          <xs:element minOccurs="0" name="codeSet" type="xs:string"/>
          <xs:element minOccurs="0" name="createdDate" type="xs:string"/>
          <xs:element minOccurs="0" name="diagnosisCode" type="xs:string"/>
          <xs:element minOccurs="0" name="diagnosisDate" type="xs:string"/>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element name="isMasterDiagnosis" type="xs:boolean"/>
          <xs:element name="isPrimary" type="xs:boolean"/>
          <xs:element minOccurs="0" name="location" type="xs:string"/>
          <xs:element minOccurs="0" name="patientDiagnosisId" type="xs:long"/>
          <xs:element minOccurs="0" name="qualifier" type="xs:string"/>
          <xs:element minOccurs="0" name="resolutionDate" type="xs:string"/>
          <xs:element minOccurs="0" name="status" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getServerTime">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getServerTimeResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="currentServerTime" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchKeyDates">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:keyDatesSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="keyDatesSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element name="keyDateType" type="xs:int"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchKeyDatesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="keyDateList" type="tns:keyDatesBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="keyDatesBasic">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="lastCompExamDate" type="xs:string"/>
          <xs:element minOccurs="0" name="lastCompExamId" type="xs:long"/>
          <xs:element minOccurs="0" name="lastCompExamProviderId" type="xs:long"/>
          <xs:element minOccurs="0" name="lastCompExamRefreshDate" type="xs:string"/>
          <xs:element minOccurs="0" name="lastCompExamType" type="xs:string"/>
          <xs:element minOccurs="0" name="lastExamDate" type="xs:string"/>
          <xs:element minOccurs="0" name="lastExamId" type="xs:long"/>
          <xs:element minOccurs="0" name="lastExamProviderId" type="xs:long"/>
          <xs:element minOccurs="0" name="lastExamRefreshDate" type="xs:string"/>
          <xs:element minOccurs="0" name="lastExamType" type="xs:string"/>
          <xs:element minOccurs="0" name="nextApptDate" type="xs:string"/>
          <xs:element minOccurs="0" name="nextApptId" type="xs:long"/>
          <xs:element minOccurs="0" name="nextApptProviderId" type="xs:long"/>
          <xs:element minOccurs="0" name="nextApptRefreshDate" type="xs:string"/>
          <xs:element minOccurs="0" name="nextApptType" type="xs:string"/>
          <xs:element minOccurs="0" name="nextRecallDate" type="xs:string"/>
          <xs:element minOccurs="0" name="nextRecallId" type="xs:long"/>
          <xs:element minOccurs="0" name="nextRecallRefreshDate" type="xs:string"/>
          <xs:element minOccurs="0" name="nextRecallType" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPaymentItemsWithLedgerPostings">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:paymentDatesExtendedSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="paymentDatesExtendedSearchRequest">
        <xs:complexContent>
          <xs:extension base="tns:paymentExtendedSearchRequest">
            <xs:sequence>
              <xs:element minOccurs="0" name="postEndDate" type="xs:string"/>
              <xs:element minOccurs="0" name="postStartDate" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="searchPaymentItemsWithLedgerPostingsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="paymentList" type="tns:paymentWithLedgerPostings"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="paymentWithLedgerPostings">
        <xs:complexContent>
          <xs:extension base="tns:payment">
            <xs:sequence>
              <xs:element maxOccurs="unbounded" minOccurs="0" name="ledgerPostings" nillable="true" type="tns:ledgerPosting"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="ledgerPosting">
        <xs:sequence>
          <xs:element name="amount" type="xs:double"/>
          <xs:element minOccurs="0" name="details" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="postedOn" type="xs:string"/>
          <xs:element name="quantityChange" type="xs:int"/>
          <xs:element name="taxAmount" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="createAppointmentFromSlot">
        <xs:sequence>
          <xs:element minOccurs="0" name="createAppointmentFromSlotRequest" type="tns:createAppointmentFromSlotRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="createAppointmentFromSlotRequest">
        <xs:complexContent>
          <xs:extension base="tns:createAppointmentBaseRequest">
            <xs:sequence>
              <xs:element minOccurs="0" name="appointmentSlotId" type="xs:long"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType abstract="true" name="createAppointmentBaseRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="apptSubTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="apptTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="createAppointmentFromSlotResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="apptId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEmployeeIdByProviderId">
        <xs:sequence>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEmployeeIdByProviderIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="deceasePatient">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="dateOfDeath" type="xs:string"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="deceasePatientResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:patientBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchRecalls">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:RecallSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchRecallsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="recallList" type="tns:recallBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchMedicationPrescriptions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:prescriptionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchMedicationPrescriptionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="medicationPrescription" type="tns:medicationPrescription"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAllProviders">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAllProvidersResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="providerList" type="tns:provider"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="provider">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element minOccurs="0" name="npi" type="xs:string"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element name="providerType" type="xs:int"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getOffices">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getOfficesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="officeList" type="tns:office"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="office">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="address" type="tns:address"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="storeNumber" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientPhotos">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:patientPhotoSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientPhotoSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientPhotosResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientPhoto" type="tns:patientPhoto"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientPhoto">
        <xs:complexContent>
          <xs:extension base="tns:practiceFile">
            <xs:sequence>
              <xs:element minOccurs="0" name="patientId" type="xs:long"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="practiceFile">
        <xs:sequence>
          <xs:element minOccurs="0" name="file" type="tns:file"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="practiceId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="createAppointmentFromDetails">
        <xs:sequence>
          <xs:element minOccurs="0" name="createAppointmentRequest" type="tns:createAppointmentRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="createAppointmentRequest">
        <xs:complexContent>
          <xs:extension base="tns:createAppointmentBaseRequest">
            <xs:sequence>
              <xs:element minOccurs="0" name="description" type="xs:string"/>
              <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
              <xs:element minOccurs="0" name="endDate" type="xs:string"/>
              <xs:element minOccurs="0" name="officeId" type="xs:long"/>
              <xs:element minOccurs="0" name="providerId" type="xs:long"/>
              <xs:element minOccurs="0" name="startDate" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="createAppointmentFromDetailsResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="apptId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchInvoicePayments">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:paymentSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchInvoicePaymentsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="paymentList" type="tns:payment"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getInsuranceCompanies">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getInsuranceCompaniesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="companyList" type="tns:insuranceCompany"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="insuranceCompany">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="companyId" type="xs:long"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element minOccurs="0" name="payorId" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchEncounters">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:encounterSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="encounterSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="approvalEndDate" type="xs:string"/>
          <xs:element minOccurs="0" name="approvalStartDate" type="xs:string"/>
          <xs:element minOccurs="0" name="approvalStatus" type="xs:int"/>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
          <xs:element minOccurs="0" name="encounterTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="locationIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientStatus" type="xs:int"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="subTypeId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchEncountersResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="encounterList" type="tns:encounterBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="encounterBasic">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="apptSubType" type="xs:string"/>
          <xs:element minOccurs="0" name="apptSubTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="apptType" type="xs:string"/>
          <xs:element minOccurs="0" name="apptTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="encounterDate" type="xs:string"/>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="officeName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientDOB" type="xs:string"/>
          <xs:element minOccurs="0" name="patientEmail" type="xs:string"/>
          <xs:element minOccurs="0" name="patientFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientGender" type="xs:string"/>
          <xs:element minOccurs="0" name="patientHomeAddress" type="tns:address"/>
          <xs:element minOccurs="0" name="patientHomePhone" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientLastName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientMobilePhone" type="xs:string"/>
          <xs:element minOccurs="0" name="patientNickName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientPreferredPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="patientWorkPhone" type="xs:string"/>
          <xs:element minOccurs="0" name="providerFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="providerLastName" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getApptTypes">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getApptTypesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="apptTypeList" type="tns:appointmentType"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentType">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="apptSubTypes" nillable="true" type="tns:appointmentSubType"/>
          <xs:element minOccurs="0" name="apptTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="apptTypeName" type="xs:string"/>
          <xs:element name="duration" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentSubType">
        <xs:sequence>
          <xs:element minOccurs="0" name="apptSubTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="apptSubTypeName" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchAppointmentSlots">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:appointmentSlotSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentSlotSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="apptTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="officeIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="preferences" type="tns:patientSchedulingPreferences"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientSchedulingPreferences">
        <xs:sequence>
          <xs:element name="apptReminderType" type="xs:int"/>
          <xs:element name="fridayPreferredTime" type="xs:int"/>
          <xs:element name="mondayPreferredTime" type="xs:int"/>
          <xs:element name="saturdayPreferredTime" type="xs:int"/>
          <xs:element name="sundayPreferredTime" type="xs:int"/>
          <xs:element name="thursdayPreferredTime" type="xs:int"/>
          <xs:element name="tuesdayPreferredTime" type="xs:int"/>
          <xs:element name="wednesdayPreferredTime" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchAppointmentSlotsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="appointmentSlotList" type="tns:appointmentSlot"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentSlot">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="appointmentSlotId" type="xs:long"/>
          <xs:element minOccurs="0" name="employeeCredentials" type="xs:string"/>
          <xs:element minOccurs="0" name="employeeFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
          <xs:element minOccurs="0" name="employeeLastName" type="xs:string"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="officeName" type="xs:string"/>
          <xs:element minOccurs="0" name="roleId" type="xs:long"/>
          <xs:element minOccurs="0" name="roleName" type="xs:string"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchSales">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:salesSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="salesSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="itemTypes" nillable="true" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="officeIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="payorInsuranceId" type="xs:long"/>
          <xs:element minOccurs="0" name="payorPatientId" type="xs:long"/>
          <xs:element name="payorType" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="productCategoryIds" nillable="true" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="productIds" nillable="true" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="providerIds" nillable="true" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="serviceIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchSalesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="salesList" type="tns:salesItem"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="salesItem">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="adjustmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="adjustmentType" type="xs:int"/>
          <xs:element minOccurs="0" name="adjustmentTypeString" type="xs:string"/>
          <xs:element name="adjustments" type="xs:double"/>
          <xs:element minOccurs="0" name="brandId" type="xs:long"/>
          <xs:element minOccurs="0" name="brandName" type="xs:string"/>
          <xs:element minOccurs="0" name="categoryId" type="xs:long"/>
          <xs:element minOccurs="0" name="categoryName" type="xs:string"/>
          <xs:element minOccurs="0" name="collectionId" type="xs:long"/>
          <xs:element minOccurs="0" name="collectionName" type="xs:string"/>
          <xs:element name="discounts" type="xs:double"/>
          <xs:element name="gross" type="xs:double"/>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="itemCode" type="xs:string"/>
          <xs:element minOccurs="0" name="itemDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="itemId" type="xs:long"/>
          <xs:element minOccurs="0" name="itemTaxId" type="xs:long"/>
          <xs:element minOccurs="0" name="itemTaxName" type="xs:string"/>
          <xs:element minOccurs="0" name="itemType" type="xs:int"/>
          <xs:element minOccurs="0" name="itemTypeString" type="xs:string"/>
          <xs:element minOccurs="0" name="manufacturerId" type="xs:long"/>
          <xs:element minOccurs="0" name="manufacturerName" type="xs:string"/>
          <xs:element name="net" type="xs:double"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientLastName" type="xs:string"/>
          <xs:element minOccurs="0" name="payorEntityId" type="xs:long"/>
          <xs:element minOccurs="0" name="payorId" type="xs:long"/>
          <xs:element minOccurs="0" name="payorName" type="xs:string"/>
          <xs:element minOccurs="0" name="payorType" type="xs:int"/>
          <xs:element minOccurs="0" name="payorTypeString" type="xs:string"/>
          <xs:element minOccurs="0" name="postedOn" type="xs:string"/>
          <xs:element minOccurs="0" name="practiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="productId" type="xs:long"/>
          <xs:element minOccurs="0" name="productUPC" type="xs:string"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="providerName" type="xs:string"/>
          <xs:element name="quantity" type="xs:int"/>
          <xs:element minOccurs="0" name="respPersonFirstName" type="xs:string"/>
          <xs:element minOccurs="0" name="respPersonId" type="xs:long"/>
          <xs:element minOccurs="0" name="respPersonLastName" type="xs:string"/>
          <xs:element minOccurs="0" name="serviceDate" type="xs:string"/>
          <xs:element minOccurs="0" name="serviceId" type="xs:long"/>
          <xs:element name="taxes" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientsLimited">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:limitedPatientSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="limitedPatientSearchRequest">
        <xs:sequence>
          <xs:element name="activeOnly" type="xs:boolean"/>
          <xs:element minOccurs="0" name="dob" type="xs:string"/>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientsLimitedResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientList" type="tns:patientBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updateOrderStatus">
        <xs:sequence>
          <xs:element minOccurs="0" name="orderStatusUpdateRequest" type="tns:orderStatusUpdateRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderStatusUpdateRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="newStatus" type="xs:int"/>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updateOrderStatusResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="rescheduleAppointmentFromDetails">
        <xs:sequence>
          <xs:element minOccurs="0" name="rescheduleAppointmentRequest" type="tns:rescheduleAppointmentRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="rescheduleAppointmentRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element name="isCopyInsVerification" type="xs:boolean"/>
          <xs:element name="isEmailPatient" type="xs:boolean"/>
          <xs:element name="isPatientInitiated" type="xs:boolean"/>
          <xs:element minOccurs="0" name="newAppointment" type="tns:createAppointmentRequest"/>
          <xs:element minOccurs="0" name="reason" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="rescheduleAppointmentFromDetailsResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="apptId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchTodaysInProgressEncounters">
        <xs:sequence>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchTodaysInProgressEncountersResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="encounterList" type="tns:encounterBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAppointmentById">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAppointmentByIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointment" type="tns:appointmentBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentBasic">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="apptDate" type="xs:string"/>
          <xs:element name="apptLength" type="xs:int"/>
          <xs:element minOccurs="0" name="apptNote" type="xs:string"/>
          <xs:element minOccurs="0" name="apptSubType" type="xs:string"/>
          <xs:element minOccurs="0" name="apptSubTypeId" type="xs:long"/>
          <xs:element minOccurs="0" name="apptType" type="xs:string"/>
          <xs:element minOccurs="0" name="apptTypeId" type="xs:long"/>
          <xs:element name="confirmed" type="xs:boolean"/>
          <xs:element minOccurs="0" name="lastUpdated" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchScheduleItems">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:scheduleItemSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="scheduleItemSearchRequest">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="employeeIds" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="itemIds" nillable="true" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="itemStatuses" nillable="true" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="itemTypes" nillable="true" type="xs:int"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchScheduleItemsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="scheduleItemList" type="tns:scheduleItem"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="scheduleItem">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="createdOn" type="xs:string"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element name="duration" type="xs:int"/>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element name="isRecurring" type="xs:boolean"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="roleId" type="xs:long"/>
          <xs:element minOccurs="0" name="roleName" type="xs:string"/>
          <xs:element minOccurs="0" name="scheduleItemId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="summary" type="xs:string"/>
          <xs:element name="type" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedOn" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updatePatientCommunicationPreferences">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="commPreferences" type="tns:patientCommunicationPreferenceUpdate"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientCommunicationPreferenceUpdate">
        <xs:sequence>
          <xs:element name="changeMask" type="xs:int"/>
          <xs:element name="doChangeOptIn" type="xs:boolean"/>
          <xs:element name="mask" type="xs:int"/>
          <xs:element name="optIn" type="xs:int"/>
          <xs:element name="preferenceType" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updatePatientCommunicationPreferencesResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEmployees">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEmployeesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="employeeList" type="tns:employee"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="employee">
        <xs:sequence>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
          <xs:element minOccurs="0" name="employeePersonId" type="xs:long"/>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatients">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:patientSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientSearchRequest">
        <xs:sequence>
          <xs:element name="activeOnly" type="xs:boolean"/>
          <xs:element minOccurs="0" name="dob" type="xs:string"/>
          <xs:element minOccurs="0" name="firstName" type="xs:string"/>
          <xs:element minOccurs="0" name="lastName" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="phone" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientList" type="tns:patientBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientById">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientByIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:patientBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="cancelAppointment">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element name="patientInitiated" type="xs:boolean"/>
          <xs:element name="emailPatient" type="xs:boolean"/>
          <xs:element minOccurs="0" name="reason" type="xs:string"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="cancelAppointmentResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientInsuranceTypes">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientInsuranceTypesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="insuranceType" type="tns:insuranceType"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="insuranceType">
        <xs:sequence>
          <xs:element name="active" type="xs:boolean"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchTransactionsV2">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:transactionExtendedSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="transactionExtendedSearchRequest">
        <xs:complexContent>
          <xs:extension base="tns:transactionSearchRequest">
            <xs:sequence>
              <xs:element minOccurs="0" name="serviceEndDate" type="xs:string"/>
              <xs:element minOccurs="0" name="serviceStartDate" type="xs:string"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="searchTransactionsV2Response">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="transactionList" type="tns:transactionWithPayor"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getProviderIdByEmployeeId">
        <xs:sequence>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getProviderIdByEmployeeIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getKeyDatesForPatient">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getKeyDatesForPatientResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:keyDatesBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchServices">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:serviceSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="serviceSearchRequest">
        <xs:sequence>
          <xs:element name="activeOnly" type="xs:boolean"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchServicesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="serviceList" type="tns:serviceBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="serviceBasic">
        <xs:sequence>
          <xs:element name="active" type="xs:boolean"/>
          <xs:element name="additionalProperties">
            <xs:complexType>
              <xs:sequence>
                <xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
                  <xs:complexType>
                    <xs:sequence>
                      <xs:element minOccurs="0" name="key" type="xs:string"/>
                      <xs:element minOccurs="0" name="value" type="xs:string"/>
                    </xs:sequence>
                  </xs:complexType>
                </xs:element>
              </xs:sequence>
            </xs:complexType>
          </xs:element>
          <xs:element minOccurs="0" name="commonDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="fullName" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="invoiceDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="longDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element name="price" type="xs:double"/>
          <xs:element name="serviceType" type="xs:int"/>
          <xs:element minOccurs="0" name="shortDescription" type="xs:string"/>
          <xs:element minOccurs="0" name="taxName" type="xs:string"/>
          <xs:element name="taxRate" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAccountSummaryWithInsurance">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAccountSummaryWithInsuranceResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="tns:patientInsuranceAccountSummary"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientInsuranceAccountSummary">
        <xs:complexContent>
          <xs:extension base="tns:patientAccountSummary">
            <xs:sequence>
              <xs:element name="collectionsBalance" type="xs:double"/>
              <xs:element minOccurs="0" name="family" type="tns:patientFamilyAccountSummary"/>
              <xs:element name="insBalance" type="xs:double"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="patientAccountSummary">
        <xs:sequence>
          <xs:element name="balance" type="xs:double"/>
          <xs:element name="credit" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientFamilyAccountSummary">
        <xs:sequence>
          <xs:element name="familyBalance" type="xs:double"/>
          <xs:element name="familyCollections" type="xs:double"/>
          <xs:element name="familyCredit" type="xs:double"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchClaims">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:claimSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="claimSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="claimEndDate" type="xs:string"/>
          <xs:element minOccurs="0" name="claimId" type="xs:long"/>
          <xs:element minOccurs="0" name="claimProcessingMechanism" type="xs:int"/>
          <xs:element minOccurs="0" name="claimProcessingStatus" type="xs:int"/>
          <xs:element minOccurs="0" name="claimStartDate" type="xs:string"/>
          <xs:element minOccurs="0" name="claimSubmittedEndDate" type="xs:string"/>
          <xs:element minOccurs="0" name="claimSubmittedStartDate" type="xs:string"/>
          <xs:element minOccurs="0" name="insuranceCompanyId" type="xs:long"/>
          <xs:element minOccurs="0" name="invoiceEndDate" type="xs:string"/>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="invoiceStartDate" type="xs:string"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientName" type="xs:string"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchClaimsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="claims" type="tns:insuranceClaim"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="insuranceClaim">
        <xs:sequence>
          <xs:element minOccurs="0" name="claimDate" type="xs:string"/>
          <xs:element name="claimSubmissionMechanism" type="xs:int"/>
          <xs:element minOccurs="0" name="claimSubmitDate" type="xs:string"/>
          <xs:element minOccurs="0" name="externalId" type="xs:string"/>
          <xs:element minOccurs="0" name="externalMessage" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="insuranceClaimProcessorName" type="xs:string"/>
          <xs:element minOccurs="0" name="invoiceId" type="xs:long"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element name="processingStatus" type="xs:int"/>
          <xs:element name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchOrders">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:orderSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="orderSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="masterProcessorId" type="xs:long"/>
          <xs:element name="notNotifiedOnly" type="xs:boolean"/>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
          <xs:element minOccurs="0" name="orderType" type="xs:int"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element name="shipToType" type="xs:int"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element name="statusCode" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="statusList" nillable="true" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
          <xs:element minOccurs="0" name="vendorName" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchOrdersResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="orderList" type="tns:orderBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchProducts">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:productSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="productSearchRequest">
        <xs:sequence>
          <xs:element name="activeOnly" type="xs:boolean"/>
          <xs:element minOccurs="0" name="category" type="xs:long"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="categoryList" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="locationProductId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchProductsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="productList" type="tns:productBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAppointmentDetailById">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAppointmentDetailByIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointment" type="tns:appointmentDetail"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentDetail">
        <xs:complexContent>
          <xs:extension base="tns:appointmentBasic">
            <xs:sequence>
              <xs:element minOccurs="0" name="office" type="tns:office"/>
              <xs:element minOccurs="0" name="patient" type="tns:patientBasic"/>
              <xs:element minOccurs="0" name="provider" type="tns:provider"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="getPatientSchedulingPreferences">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientSchedulingPreferencesResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientSchedulingPreferences" type="tns:patientSchedulingPreferences"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchAppointments">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:appointmentSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="appointmentSearchRequest">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="apptStatusList" nillable="true" type="xs:int"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="apptTypeList" nillable="true" type="xs:long"/>
          <xs:element minOccurs="0" name="endDate" type="xs:string"/>
          <xs:element minOccurs="0" name="officeId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="providerId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:string"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchAppointmentsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="appointmentList" type="tns:appointmentBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getOrderDetailById">
        <xs:sequence>
          <xs:element minOccurs="0" name="orderId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getOrderDetailByIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="order" type="tns:orderDetail"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="echo">
        <xs:sequence>
          <xs:element minOccurs="0" name="echoRequest" type="xs:string"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="echoResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="echoResponse" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchRefractions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:refractionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="refractionSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element minOccurs="0" name="endDate" type="xs:dateTime"/>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="masterIds" nillable="true" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="startDate" type="xs:dateTime"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchRefractionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="refraction" type="tns:refraction"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="refraction">
        <xs:sequence>
          <xs:element minOccurs="0" name="addVisualAcuity" type="xs:string"/>
          <xs:element minOccurs="0" name="addVisualAcuityModifier" type="xs:string"/>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element minOccurs="0" name="instructions" type="xs:string"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
          <xs:element minOccurs="0" name="od" type="tns:refractionEye"/>
          <xs:element minOccurs="0" name="os" type="tns:refractionEye"/>
          <xs:element minOccurs="0" name="ouVisualAcuity" type="xs:string"/>
          <xs:element minOccurs="0" name="ouVisualAcuityModifier" type="xs:string"/>
          <xs:element minOccurs="0" name="testDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="refractionEye">
        <xs:sequence>
          <xs:element minOccurs="0" name="axis" type="xs:string"/>
          <xs:element minOccurs="0" name="balanced" type="xs:boolean"/>
          <xs:element minOccurs="0" name="cylinder" type="xs:string"/>
          <xs:element minOccurs="0" name="horizontalPrism" type="xs:string"/>
          <xs:element minOccurs="0" name="horizontalPrismOrientation" type="xs:string"/>
          <xs:element minOccurs="0" name="intermediateAdd" type="xs:string"/>
          <xs:element minOccurs="0" name="nearAdd" type="xs:string"/>
          <xs:element minOccurs="0" name="prism" type="xs:string"/>
          <xs:element minOccurs="0" name="prismOrientation" type="xs:string"/>
          <xs:element minOccurs="0" name="sphere" type="xs:string"/>
          <xs:element minOccurs="0" name="visualAcuity" type="xs:string"/>
          <xs:element minOccurs="0" name="visualAcuityModifier" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPayments">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:paymentExtendedSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPaymentsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="paymentList" type="tns:payment"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientInsuranceInfo">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientInsuranceInfoResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="insuranceInfo" type="tns:insurance"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="insurance">
        <xs:sequence>
          <xs:element minOccurs="0" name="copays" type="tns:coPays"/>
          <xs:element minOccurs="0" name="groupNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="individualCopays" type="tns:coPays"/>
          <xs:element minOccurs="0" name="insuranceCompanyName" type="xs:string"/>
          <xs:element minOccurs="0" name="insuranceType" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="policyNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="priority" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="coPays">
        <xs:sequence>
          <xs:element minOccurs="0" name="authorizationDate" type="xs:string"/>
          <xs:element minOccurs="0" name="authorizationNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="contactLensAllowance" type="xs:double"/>
          <xs:element minOccurs="0" name="contactLensBenefitEligible" type="xs:boolean"/>
          <xs:element minOccurs="0" name="contactLensBenefitResetDate" type="xs:string"/>
          <xs:element minOccurs="0" name="contactLensFitting" type="xs:double"/>
          <xs:element minOccurs="0" name="contactLensFittingEligible" type="xs:boolean"/>
          <xs:element minOccurs="0" name="contactLensFittingResetDate" type="xs:string"/>
          <xs:element minOccurs="0" name="frameBenefitEligible" type="xs:boolean"/>
          <xs:element minOccurs="0" name="frameBenefitResetDate" type="xs:string"/>
          <xs:element minOccurs="0" name="lensBenefitEligible" type="xs:boolean"/>
          <xs:element minOccurs="0" name="lensBenefitResetDate" type="xs:string"/>
          <xs:element minOccurs="0" name="materials" type="xs:double"/>
          <xs:element minOccurs="0" name="maximumFrameAllowance" type="xs:double"/>
          <xs:element minOccurs="0" name="medicalExam" type="xs:double"/>
          <xs:element minOccurs="0" name="minimumFrameAllowance" type="xs:double"/>
          <xs:element minOccurs="0" name="officeVisit" type="xs:double"/>
          <xs:element minOccurs="0" name="routineExam" type="xs:double"/>
          <xs:element minOccurs="0" name="routineExamEligible" type="xs:boolean"/>
          <xs:element minOccurs="0" name="routineExamResetDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchAppointmentsWithDetail">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:appointmentSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchAppointmentsWithDetailResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="appointmentList" type="tns:appointmentDetail"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAllEmployees">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getAllEmployeesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="employeeList" type="tns:employee"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchOrderDetail">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:orderSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchOrderDetailResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="orderDetailList" type="tns:orderDetail"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientBalances">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientId" type="tns:patientBalanceSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientBalanceSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="hasBalance" type="xs:boolean"/>
          <xs:element minOccurs="0" name="locationId" type="xs:long"/>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientBalancesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientBalanceList" type="tns:patientBalance"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientBalance">
        <xs:sequence>
          <xs:element name="balance" type="xs:double"/>
          <xs:element name="credit" type="xs:double"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="updatedDate" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="readinessCheck">
        <xs:sequence/>
      </xs:complexType>
      <xs:complexType name="readinessCheckResponse">
        <xs:sequence/>
      </xs:complexType>
      <xs:complexType name="searchEyeglassPrescriptions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:prescriptionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchEyeglassPrescriptionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="eyeglassPrescriptionList" type="tns:eyeglassPrescription"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEmployeeOffices">
        <xs:sequence>
          <xs:element minOccurs="0" name="employeeId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEmployeeOfficesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="officeList" type="tns:office"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="addPatient">
        <xs:sequence>
          <xs:element minOccurs="0" name="patient" type="tns:patientMinimal"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="addPatientResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="newPatientId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientPhotoContent">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientPhotoId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientPhotoContentResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="return" type="xs:base64Binary"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchExternalMedicationPrescriptions">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:prescriptionSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchExternalMedicationPrescriptionsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="medicationPrescription" type="tns:medicationPrescription"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchKeyDatesDetail">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:keyDatesSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchKeyDatesDetailResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="return" type="tns:keyDatesDetail"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="keyDatesDetail">
        <xs:complexContent>
          <xs:extension base="tns:keyDatesBasic">
            <xs:sequence>
              <xs:element minOccurs="0" name="patient" type="tns:patientBasic"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="searchPaymentsWithLedgerPostings">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:paymentDatesExtendedSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPaymentsWithLedgerPostingsResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="paymentList" type="tns:paymentWithLedgerPostings"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientInsurancePriorities">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getPatientInsurancePrioritiesResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="insurancePriority" type="tns:insurancePriority"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="insurancePriority">
        <xs:sequence>
          <xs:element name="active" type="xs:boolean"/>
          <xs:element minOccurs="0" name="description" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="name" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="verifyPatientUserNameAvailable">
        <xs:sequence>
          <xs:element minOccurs="0" name="userName" type="xs:string"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="verifyPatientUserNameAvailableResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="available" type="xs:boolean"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientInsuranceInfo">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:PatientInsuranceSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="PatientInsuranceSearchRequest">
        <xs:sequence>
          <xs:element minOccurs="0" name="pageNumber" type="xs:int"/>
          <xs:element minOccurs="0" name="pageSize" type="xs:int"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="updatedSince" type="xs:string"/>
          <xs:element minOccurs="0" name="status" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientInsuranceInfoResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="insuranceInfo" type="tns:patientInsurance"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientInsurance">
        <xs:sequence>
          <xs:element minOccurs="0" name="coPays" type="tns:coPays"/>
          <xs:element minOccurs="0" name="createdOn" type="xs:string"/>
          <xs:element minOccurs="0" name="deductible" type="xs:double"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="insuranceType" type="xs:long"/>
          <xs:element minOccurs="0" name="patientBenefits" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="policy" type="tns:patientInsurancePolicy"/>
          <xs:element minOccurs="0" name="policyHolderRelationship" type="xs:int"/>
          <xs:element minOccurs="0" name="policyNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="priorityId" type="xs:long"/>
          <xs:element minOccurs="0" name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="updatedOn" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientInsurancePolicy">
        <xs:sequence>
          <xs:element minOccurs="0" name="coInsurancePct" type="xs:double"/>
          <xs:element minOccurs="0" name="coPays" type="tns:coPays"/>
          <xs:element minOccurs="0" name="effectiveDate" type="xs:string"/>
          <xs:element minOccurs="0" name="familyDeductible" type="xs:double"/>
          <xs:element minOccurs="0" name="feeScheduleId" type="xs:long"/>
          <xs:element minOccurs="0" name="groupNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="id" type="xs:long"/>
          <xs:element minOccurs="0" name="insCompanyId" type="xs:long"/>
          <xs:element minOccurs="0" name="planName" type="xs:string"/>
          <xs:element minOccurs="0" name="policyBenefits" type="xs:string"/>
          <xs:element minOccurs="0" name="policyHolderPatientId" type="xs:long"/>
          <xs:element minOccurs="0" name="referralRequired" type="xs:boolean"/>
          <xs:element minOccurs="0" name="rxBinNumber" type="xs:string"/>
          <xs:element minOccurs="0" name="rxPcnNumber" type="xs:string"/>
          <xs:element name="status" type="xs:int"/>
          <xs:element minOccurs="0" name="tpaId" type="xs:long"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getProviders">
        <xs:sequence>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getProvidersResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="providerList" type="tns:provider"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEncounterById">
        <xs:sequence>
          <xs:element minOccurs="0" name="encounterId" type="xs:long"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="getEncounterByIdResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="encounterList" type="tns:encounterBasic"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updatePatientLogin">
        <xs:sequence>
          <xs:element minOccurs="0" name="patientLogin" type="tns:patientLogin"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientLogin">
        <xs:sequence>
          <xs:element minOccurs="0" name="newPassword" type="xs:string"/>
          <xs:element minOccurs="0" name="oldPassword" type="xs:string"/>
          <xs:element minOccurs="0" name="patientId" type="xs:long"/>
          <xs:element minOccurs="0" name="userName" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="updatePatientLoginResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="confirmAppointment">
        <xs:sequence>
          <xs:element minOccurs="0" name="appointmentId" type="xs:long"/>
          <xs:element minOccurs="0" name="comment" type="xs:string"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="confirmAppointmentResponse">
        <xs:sequence>
          <xs:element minOccurs="0" name="result" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientsWithReferral">
        <xs:sequence>
          <xs:element minOccurs="0" name="searchRequest" type="tns:patientSearchRequest"/>
          <xs:element minOccurs="0" name="userId" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="searchPatientsWithReferralResponse">
        <xs:sequence>
          <xs:element maxOccurs="unbounded" minOccurs="0" name="patientList" type="tns:patientWithReferral"/>
        </xs:sequence>
      </xs:complexType>
      <xs:complexType name="patientWithReferral">
        <xs:complexContent>
          <xs:extension base="tns:patientBasic">
            <xs:sequence>
              <xs:element minOccurs="0" name="referral" type="tns:patientReferral"/>
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:complexType name="patientReferral">
        <xs:sequence>
          <xs:element minOccurs="0" name="comments" type="xs:string"/>
          <xs:element minOccurs="0" name="referralDate" type="xs:string"/>
          <xs:element minOccurs="0" name="referringPatient" type="tns:patientBasic"/>
          <xs:element minOccurs="0" name="referringProvider" type="tns:provider"/>
          <xs:element minOccurs="0" name="rewardDate" type="xs:string"/>
          <xs:element minOccurs="0" name="rewardProgram" type="xs:string"/>
          <xs:element minOccurs="0" name="sourceName" type="xs:string"/>
          <xs:element minOccurs="0" name="sourceType" type="xs:int"/>
        </xs:sequence>
      </xs:complexType>
      <xs:element name="WebServiceException" type="tns:WebServiceException"/>
      <xs:complexType name="WebServiceException">
        <xs:sequence>
          <xs:element minOccurs="0" name="details" type="xs:string"/>
          <xs:element minOccurs="0" name="errorCode" type="xs:string"/>
          <xs:element minOccurs="0" name="errorMessage" type="xs:string"/>
        </xs:sequence>
      </xs:complexType>
    </xs:schema>
  </wsdl:types>
  <wsdl:message name="searchPaymentItems">
    <wsdl:part element="tns:searchPaymentItems" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchScheduleItemsResponse">
    <wsdl:part element="tns:searchScheduleItemsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="uploadPatientFilesToFolder">
    <wsdl:part element="tns:uploadPatientFilesToFolder" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getApptTypesResponse">
    <wsdl:part element="tns:getApptTypesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="setPatientNotified">
    <wsdl:part element="tns:setPatientNotified" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPaymentsWithLedgerPostingsResponse">
    <wsdl:part element="tns:searchPaymentsWithLedgerPostingsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTransactionsResponse">
    <wsdl:part element="tns:searchTransactionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="createAppointmentFromDetailsResponse">
    <wsdl:part element="tns:createAppointmentFromDetailsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updatePatient">
    <wsdl:part element="tns:updatePatient" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAppointmentByIdResponse">
    <wsdl:part element="tns:getAppointmentByIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getKeyDatesForPatientResponse">
    <wsdl:part element="tns:getKeyDatesForPatientResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientTransactions">
    <wsdl:part element="tns:searchPatientTransactions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getInsuranceCompaniesResponse">
    <wsdl:part element="tns:getInsuranceCompaniesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientsLimitedResponse">
    <wsdl:part element="tns:searchPatientsLimitedResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="addPatientResponse">
    <wsdl:part element="tns:addPatientResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="activatePatientResponse">
    <wsdl:part element="tns:activatePatientResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPaymentItemsWithLedgerPostings">
    <wsdl:part element="tns:searchPaymentItemsWithLedgerPostings" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchSalesResponse">
    <wsdl:part element="tns:searchSalesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="deceasePatient">
    <wsdl:part element="tns:deceasePatient" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchRecalls">
    <wsdl:part element="tns:searchRecalls" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getOffices">
    <wsdl:part element="tns:getOffices" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="createAppointmentFromDetails">
    <wsdl:part element="tns:createAppointmentFromDetails" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchInvoicePayments">
    <wsdl:part element="tns:searchInvoicePayments" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientsWithReferralResponse">
    <wsdl:part element="tns:searchPatientsWithReferralResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getInsuranceCompanies">
    <wsdl:part element="tns:getInsuranceCompanies" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getProvidersResponse">
    <wsdl:part element="tns:getProvidersResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchEncounters">
    <wsdl:part element="tns:searchEncounters" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchAppointmentsResponse">
    <wsdl:part element="tns:searchAppointmentsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getApptTypes">
    <wsdl:part element="tns:getApptTypes" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchAppointmentSlots">
    <wsdl:part element="tns:searchAppointmentSlots" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchSales">
    <wsdl:part element="tns:searchSales" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientsLimited">
    <wsdl:part element="tns:searchPatientsLimited" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updateOrderStatus">
    <wsdl:part element="tns:updateOrderStatus" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="rescheduleAppointmentFromDetails">
    <wsdl:part element="tns:rescheduleAppointmentFromDetails" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchScheduleItems">
    <wsdl:part element="tns:searchScheduleItems" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEmployees">
    <wsdl:part element="tns:getEmployees" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchProductsResponse">
    <wsdl:part element="tns:searchProductsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="deactivatePatientResponse">
    <wsdl:part element="tns:deactivatePatientResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientById">
    <wsdl:part element="tns:getPatientById" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updatePatientResponse">
    <wsdl:part element="tns:updatePatientResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEmployeesResponse">
    <wsdl:part element="tns:getEmployeesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientInsuranceTypesResponse">
    <wsdl:part element="tns:getPatientInsuranceTypesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPaymentItemsResponse">
    <wsdl:part element="tns:searchPaymentItemsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="cancelAppointmentResponse">
    <wsdl:part element="tns:cancelAppointmentResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="echoResponse">
    <wsdl:part element="tns:echoResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getKeyDatesForPatient">
    <wsdl:part element="tns:getKeyDatesForPatient" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAccountSummaryWithInsurance">
    <wsdl:part element="tns:getAccountSummaryWithInsurance" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchClaims">
    <wsdl:part element="tns:searchClaims" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchInvoicePaymentsResponse">
    <wsdl:part element="tns:searchInvoicePaymentsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAppointmentDetailById">
    <wsdl:part element="tns:getAppointmentDetailById" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientInsuranceInfoResponse">
    <wsdl:part element="tns:searchPatientInsuranceInfoResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientSchedulingPreferences">
    <wsdl:part element="tns:getPatientSchedulingPreferences" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getOrderDetailById">
    <wsdl:part element="tns:getOrderDetailById" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="createAppointmentFromSlotResponse">
    <wsdl:part element="tns:createAppointmentFromSlotResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="echo">
    <wsdl:part element="tns:echo" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="rescheduleAppointmentFromDetailsResponse">
    <wsdl:part element="tns:rescheduleAppointmentFromDetailsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchRefractionsResponse">
    <wsdl:part element="tns:searchRefractionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchRefractions">
    <wsdl:part element="tns:searchRefractions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPayments">
    <wsdl:part element="tns:searchPayments" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getRecallByIdResponse">
    <wsdl:part element="tns:getRecallByIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPaymentsResponse">
    <wsdl:part element="tns:searchPaymentsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="uploadPatientFilesToFolderResponse">
    <wsdl:part element="tns:uploadPatientFilesToFolderResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAllEmployees">
    <wsdl:part element="tns:getAllEmployees" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientBalancesResponse">
    <wsdl:part element="tns:searchPatientBalancesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEncounterByIdResponse">
    <wsdl:part element="tns:getEncounterByIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updatePatientLoginResponse">
    <wsdl:part element="tns:updatePatientLoginResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getInvoiceNotesResponse">
    <wsdl:part element="tns:getInvoiceNotesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientPhotosResponse">
    <wsdl:part element="tns:searchPatientPhotosResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchAppointmentsWithDetailResponse">
    <wsdl:part element="tns:searchAppointmentsWithDetailResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchEyeglassPrescriptions">
    <wsdl:part element="tns:searchEyeglassPrescriptions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getOrderDetailByIdResponse">
    <wsdl:part element="tns:getOrderDetailByIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEmployeeOffices">
    <wsdl:part element="tns:getEmployeeOffices" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientInsuranceInfoResponse">
    <wsdl:part element="tns:getPatientInsuranceInfoResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchExternalMedicationPrescriptions">
    <wsdl:part element="tns:searchExternalMedicationPrescriptions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEmployeeOfficesResponse">
    <wsdl:part element="tns:getEmployeeOfficesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchDeletedRecallsResponse">
    <wsdl:part element="tns:searchDeletedRecallsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAppointmentDetailByIdResponse">
    <wsdl:part element="tns:getAppointmentDetailByIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getProviders">
    <wsdl:part element="tns:getProviders" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEncounterById">
    <wsdl:part element="tns:getEncounterById" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updatePatientLogin">
    <wsdl:part element="tns:updatePatientLogin" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchServicesResponse">
    <wsdl:part element="tns:searchServicesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="confirmAppointment">
    <wsdl:part element="tns:confirmAppointment" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientsWithReferral">
    <wsdl:part element="tns:searchPatientsWithReferral" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchOrderDetailResponse">
    <wsdl:part element="tns:searchOrderDetailResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="deactivatePatient">
    <wsdl:part element="tns:deactivatePatient" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchOrdersResponse">
    <wsdl:part element="tns:searchOrdersResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchExternalMedicationPrescriptionsResponse">
    <wsdl:part element="tns:searchExternalMedicationPrescriptionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getInvoiceNotes">
    <wsdl:part element="tns:getInvoiceNotes" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getRecallById">
    <wsdl:part element="tns:getRecallById" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchContactLensPrescriptions">
    <wsdl:part element="tns:searchContactLensPrescriptions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="activatePatient">
    <wsdl:part element="tns:activatePatient" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientDiagnoses">
    <wsdl:part element="tns:searchPatientDiagnoses" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEmployeeIdByProviderIdResponse">
    <wsdl:part element="tns:getEmployeeIdByProviderIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchMedicationPrescriptionsResponse">
    <wsdl:part element="tns:searchMedicationPrescriptionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchEncountersResponse">
    <wsdl:part element="tns:searchEncountersResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchDeletedRecalls">
    <wsdl:part element="tns:searchDeletedRecalls" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTransactions">
    <wsdl:part element="tns:searchTransactions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getServerTimeResponse">
    <wsdl:part element="tns:getServerTimeResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTransactionsWithDiagnoses">
    <wsdl:part element="tns:searchTransactionsWithDiagnoses" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getServerTime">
    <wsdl:part element="tns:getServerTime" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchKeyDates">
    <wsdl:part element="tns:searchKeyDates" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getOfficesResponse">
    <wsdl:part element="tns:getOfficesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientsResponse">
    <wsdl:part element="tns:searchPatientsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientTransactionsResponse">
    <wsdl:part element="tns:searchPatientTransactionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="createAppointmentFromSlot">
    <wsdl:part element="tns:createAppointmentFromSlot" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getEmployeeIdByProviderId">
    <wsdl:part element="tns:getEmployeeIdByProviderId" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchMedicationPrescriptions">
    <wsdl:part element="tns:searchMedicationPrescriptions" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAllProviders">
    <wsdl:part element="tns:getAllProviders" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="verifyPatientUserNameAvailableResponse">
    <wsdl:part element="tns:verifyPatientUserNameAvailableResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientPhotos">
    <wsdl:part element="tns:searchPatientPhotos" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAllEmployeesResponse">
    <wsdl:part element="tns:getAllEmployeesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientPhotoContentResponse">
    <wsdl:part element="tns:getPatientPhotoContentResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchKeyDatesDetailResponse">
    <wsdl:part element="tns:searchKeyDatesDetailResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="deceasePatientResponse">
    <wsdl:part element="tns:deceasePatientResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTodaysInProgressEncounters">
    <wsdl:part element="tns:searchTodaysInProgressEncounters" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAppointmentById">
    <wsdl:part element="tns:getAppointmentById" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updatePatientCommunicationPreferences">
    <wsdl:part element="tns:updatePatientCommunicationPreferences" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchEyeglassPrescriptionsResponse">
    <wsdl:part element="tns:searchEyeglassPrescriptionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTransactionsV2Response">
    <wsdl:part element="tns:searchTransactionsV2Response" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTransactionsWithDiagnosesResponse">
    <wsdl:part element="tns:searchTransactionsWithDiagnosesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="WebServiceException">
    <wsdl:part element="tns:WebServiceException" name="WebServiceException"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatients">
    <wsdl:part element="tns:searchPatients" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getProviderIdByEmployeeIdResponse">
    <wsdl:part element="tns:getProviderIdByEmployeeIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="cancelAppointment">
    <wsdl:part element="tns:cancelAppointment" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientInsuranceTypes">
    <wsdl:part element="tns:getPatientInsuranceTypes" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTransactionsV2">
    <wsdl:part element="tns:searchTransactionsV2" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getProviderIdByEmployeeId">
    <wsdl:part element="tns:getProviderIdByEmployeeId" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchServices">
    <wsdl:part element="tns:searchServices" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientDiagnosesResponse">
    <wsdl:part element="tns:searchPatientDiagnosesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientInsurancePrioritiesResponse">
    <wsdl:part element="tns:getPatientInsurancePrioritiesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchOrders">
    <wsdl:part element="tns:searchOrders" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchProducts">
    <wsdl:part element="tns:searchProducts" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchAppointments">
    <wsdl:part element="tns:searchAppointments" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updatePatientCommunicationPreferencesResponse">
    <wsdl:part element="tns:updatePatientCommunicationPreferencesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="setPatientNotifiedResponse">
    <wsdl:part element="tns:setPatientNotifiedResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientByIdResponse">
    <wsdl:part element="tns:getPatientByIdResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="updateOrderStatusResponse">
    <wsdl:part element="tns:updateOrderStatusResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAllProvidersResponse">
    <wsdl:part element="tns:getAllProvidersResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchTodaysInProgressEncountersResponse">
    <wsdl:part element="tns:searchTodaysInProgressEncountersResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchRecallsResponse">
    <wsdl:part element="tns:searchRecallsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientSchedulingPreferencesResponse">
    <wsdl:part element="tns:getPatientSchedulingPreferencesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchClaimsResponse">
    <wsdl:part element="tns:searchClaimsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientInsuranceInfo">
    <wsdl:part element="tns:getPatientInsuranceInfo" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="readinessCheckResponse">
    <wsdl:part element="tns:readinessCheckResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchAppointmentsWithDetail">
    <wsdl:part element="tns:searchAppointmentsWithDetail" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchAppointmentSlotsResponse">
    <wsdl:part element="tns:searchAppointmentSlotsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchContactLensPrescriptionsResponse">
    <wsdl:part element="tns:searchContactLensPrescriptionsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchOrderDetail">
    <wsdl:part element="tns:searchOrderDetail" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientBalances">
    <wsdl:part element="tns:searchPatientBalances" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchKeyDatesResponse">
    <wsdl:part element="tns:searchKeyDatesResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="readinessCheck">
    <wsdl:part element="tns:readinessCheck" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="confirmAppointmentResponse">
    <wsdl:part element="tns:confirmAppointmentResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getAccountSummaryWithInsuranceResponse">
    <wsdl:part element="tns:getAccountSummaryWithInsuranceResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="addPatient">
    <wsdl:part element="tns:addPatient" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientPhotoContent">
    <wsdl:part element="tns:getPatientPhotoContent" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchKeyDatesDetail">
    <wsdl:part element="tns:searchKeyDatesDetail" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPaymentsWithLedgerPostings">
    <wsdl:part element="tns:searchPaymentsWithLedgerPostings" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="getPatientInsurancePriorities">
    <wsdl:part element="tns:getPatientInsurancePriorities" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="verifyPatientUserNameAvailable">
    <wsdl:part element="tns:verifyPatientUserNameAvailable" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPatientInsuranceInfo">
    <wsdl:part element="tns:searchPatientInsuranceInfo" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:message name="searchPaymentItemsWithLedgerPostingsResponse">
    <wsdl:part element="tns:searchPaymentItemsWithLedgerPostingsResponse" name="parameters"></wsdl:part>
  </wsdl:message>
  <wsdl:portType name="partner">
    <wsdl:operation name="searchPaymentItems">
      <wsdl:input message="tns:searchPaymentItems" name="searchPaymentItems" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsRequest"></wsdl:input>
      <wsdl:output message="tns:searchPaymentItemsResponse" name="searchPaymentItemsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItems/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="deactivatePatient">
      <wsdl:input message="tns:deactivatePatient" name="deactivatePatient" wsam:Action="http://ws.partner.revolutionehr.com/partner/deactivatePatientRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/deactivatePatientRequest"></wsdl:input>
      <wsdl:output message="tns:deactivatePatientResponse" name="deactivatePatientResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/deactivatePatientResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/deactivatePatientResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/deactivatePatient/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="uploadPatientFilesToFolder">
      <wsdl:input message="tns:uploadPatientFilesToFolder" name="uploadPatientFilesToFolder" wsam:Action="http://ws.partner.revolutionehr.com/partner/uploadPatientFilesToFolderRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/uploadPatientFilesToFolderRequest"></wsdl:input>
      <wsdl:output message="tns:uploadPatientFilesToFolderResponse" name="uploadPatientFilesToFolderResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/uploadPatientFilesToFolderResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/uploadPatientFilesToFolderResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/uploadPatientFilesToFolder/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getInvoiceNotes">
      <wsdl:input message="tns:getInvoiceNotes" name="getInvoiceNotes" wsam:Action="http://ws.partner.revolutionehr.com/partner/getInvoiceNotesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getInvoiceNotesRequest"></wsdl:input>
      <wsdl:output message="tns:getInvoiceNotesResponse" name="getInvoiceNotesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getInvoiceNotesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getInvoiceNotesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getInvoiceNotes/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getRecallById">
      <wsdl:input message="tns:getRecallById" name="getRecallById" wsam:Action="http://ws.partner.revolutionehr.com/partner/getRecallByIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getRecallByIdRequest"></wsdl:input>
      <wsdl:output message="tns:getRecallByIdResponse" name="getRecallByIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getRecallByIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getRecallByIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getRecallById/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="setPatientNotified">
      <wsdl:input message="tns:setPatientNotified" name="setPatientNotified" wsam:Action="http://ws.partner.revolutionehr.com/partner/setPatientNotifiedRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/setPatientNotifiedRequest"></wsdl:input>
      <wsdl:output message="tns:setPatientNotifiedResponse" name="setPatientNotifiedResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/setPatientNotifiedResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/setPatientNotifiedResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/setPatientNotified/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchContactLensPrescriptions">
      <wsdl:input message="tns:searchContactLensPrescriptions" name="searchContactLensPrescriptions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchContactLensPrescriptionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchContactLensPrescriptionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchContactLensPrescriptionsResponse" name="searchContactLensPrescriptionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchContactLensPrescriptionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchContactLensPrescriptionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchContactLensPrescriptions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="activatePatient">
      <wsdl:input message="tns:activatePatient" name="activatePatient" wsam:Action="http://ws.partner.revolutionehr.com/partner/activatePatientRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/activatePatientRequest"></wsdl:input>
      <wsdl:output message="tns:activatePatientResponse" name="activatePatientResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/activatePatientResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/activatePatientResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/activatePatient/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updatePatient">
      <wsdl:input message="tns:updatePatient" name="updatePatient" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updatePatientRequest"></wsdl:input>
      <wsdl:output message="tns:updatePatientResponse" name="updatePatientResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updatePatientResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatient/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientDiagnoses">
      <wsdl:input message="tns:searchPatientDiagnoses" name="searchPatientDiagnoses" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientDiagnosesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientDiagnosesRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientDiagnosesResponse" name="searchPatientDiagnosesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientDiagnosesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientDiagnosesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientDiagnoses/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientTransactions">
      <wsdl:input message="tns:searchPatientTransactions" name="searchPatientTransactions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientTransactionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientTransactionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientTransactionsResponse" name="searchPatientTransactionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientTransactionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientTransactionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientTransactions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchDeletedRecalls">
      <wsdl:input message="tns:searchDeletedRecalls" name="searchDeletedRecalls" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchDeletedRecallsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchDeletedRecallsRequest"></wsdl:input>
      <wsdl:output message="tns:searchDeletedRecallsResponse" name="searchDeletedRecallsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchDeletedRecallsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchDeletedRecallsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchDeletedRecalls/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTransactions">
      <wsdl:input message="tns:searchTransactions" name="searchTransactions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchTransactionsResponse" name="searchTransactionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTransactionsWithDiagnoses">
      <wsdl:input message="tns:searchTransactionsWithDiagnoses" name="searchTransactionsWithDiagnoses" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsWithDiagnosesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsWithDiagnosesRequest"></wsdl:input>
      <wsdl:output message="tns:searchTransactionsWithDiagnosesResponse" name="searchTransactionsWithDiagnosesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsWithDiagnosesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsWithDiagnosesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsWithDiagnoses/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getServerTime">
      <wsdl:input message="tns:getServerTime" name="getServerTime" wsam:Action="http://ws.partner.revolutionehr.com/partner/getServerTimeRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getServerTimeRequest"></wsdl:input>
      <wsdl:output message="tns:getServerTimeResponse" name="getServerTimeResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getServerTimeResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getServerTimeResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getServerTime/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchKeyDates">
      <wsdl:input message="tns:searchKeyDates" name="searchKeyDates" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesRequest"></wsdl:input>
      <wsdl:output message="tns:searchKeyDatesResponse" name="searchKeyDatesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDates/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPaymentItemsWithLedgerPostings">
      <wsdl:input message="tns:searchPaymentItemsWithLedgerPostings" name="searchPaymentItemsWithLedgerPostings" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsWithLedgerPostingsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsWithLedgerPostingsRequest"></wsdl:input>
      <wsdl:output message="tns:searchPaymentItemsWithLedgerPostingsResponse" name="searchPaymentItemsWithLedgerPostingsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsWithLedgerPostingsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsWithLedgerPostingsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentItemsWithLedgerPostings/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="createAppointmentFromSlot">
      <wsdl:input message="tns:createAppointmentFromSlot" name="createAppointmentFromSlot" wsam:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromSlotRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromSlotRequest"></wsdl:input>
      <wsdl:output message="tns:createAppointmentFromSlotResponse" name="createAppointmentFromSlotResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromSlotResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromSlotResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromSlot/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEmployeeIdByProviderId">
      <wsdl:input message="tns:getEmployeeIdByProviderId" name="getEmployeeIdByProviderId" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeIdByProviderIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeIdByProviderIdRequest"></wsdl:input>
      <wsdl:output message="tns:getEmployeeIdByProviderIdResponse" name="getEmployeeIdByProviderIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeIdByProviderIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeIdByProviderIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeIdByProviderId/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="deceasePatient">
      <wsdl:input message="tns:deceasePatient" name="deceasePatient" wsam:Action="http://ws.partner.revolutionehr.com/partner/deceasePatientRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/deceasePatientRequest"></wsdl:input>
      <wsdl:output message="tns:deceasePatientResponse" name="deceasePatientResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/deceasePatientResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/deceasePatientResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/deceasePatient/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchRecalls">
      <wsdl:input message="tns:searchRecalls" name="searchRecalls" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchRecallsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchRecallsRequest"></wsdl:input>
      <wsdl:output message="tns:searchRecallsResponse" name="searchRecallsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchRecallsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchRecallsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchRecalls/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchMedicationPrescriptions">
      <wsdl:input message="tns:searchMedicationPrescriptions" name="searchMedicationPrescriptions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchMedicationPrescriptionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchMedicationPrescriptionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchMedicationPrescriptionsResponse" name="searchMedicationPrescriptionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchMedicationPrescriptionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchMedicationPrescriptionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchMedicationPrescriptions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAllProviders">
      <wsdl:input message="tns:getAllProviders" name="getAllProviders" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAllProvidersRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAllProvidersRequest"></wsdl:input>
      <wsdl:output message="tns:getAllProvidersResponse" name="getAllProvidersResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAllProvidersResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAllProvidersResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAllProviders/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getOffices">
      <wsdl:input message="tns:getOffices" name="getOffices" wsam:Action="http://ws.partner.revolutionehr.com/partner/getOfficesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getOfficesRequest"></wsdl:input>
      <wsdl:output message="tns:getOfficesResponse" name="getOfficesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getOfficesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getOfficesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getOffices/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientPhotos">
      <wsdl:input message="tns:searchPatientPhotos" name="searchPatientPhotos" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientPhotosRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientPhotosRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientPhotosResponse" name="searchPatientPhotosResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientPhotosResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientPhotosResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientPhotos/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="createAppointmentFromDetails">
      <wsdl:input message="tns:createAppointmentFromDetails" name="createAppointmentFromDetails" wsam:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromDetailsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromDetailsRequest"></wsdl:input>
      <wsdl:output message="tns:createAppointmentFromDetailsResponse" name="createAppointmentFromDetailsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromDetailsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromDetailsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/createAppointmentFromDetails/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchInvoicePayments">
      <wsdl:input message="tns:searchInvoicePayments" name="searchInvoicePayments" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchInvoicePaymentsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchInvoicePaymentsRequest"></wsdl:input>
      <wsdl:output message="tns:searchInvoicePaymentsResponse" name="searchInvoicePaymentsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchInvoicePaymentsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchInvoicePaymentsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchInvoicePayments/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getInsuranceCompanies">
      <wsdl:input message="tns:getInsuranceCompanies" name="getInsuranceCompanies" wsam:Action="http://ws.partner.revolutionehr.com/partner/getInsuranceCompaniesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getInsuranceCompaniesRequest"></wsdl:input>
      <wsdl:output message="tns:getInsuranceCompaniesResponse" name="getInsuranceCompaniesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getInsuranceCompaniesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getInsuranceCompaniesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getInsuranceCompanies/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchEncounters">
      <wsdl:input message="tns:searchEncounters" name="searchEncounters" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchEncountersRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchEncountersRequest"></wsdl:input>
      <wsdl:output message="tns:searchEncountersResponse" name="searchEncountersResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchEncountersResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchEncountersResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchEncounters/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getApptTypes">
      <wsdl:input message="tns:getApptTypes" name="getApptTypes" wsam:Action="http://ws.partner.revolutionehr.com/partner/getApptTypesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getApptTypesRequest"></wsdl:input>
      <wsdl:output message="tns:getApptTypesResponse" name="getApptTypesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getApptTypesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getApptTypesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getApptTypes/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchAppointmentSlots">
      <wsdl:input message="tns:searchAppointmentSlots" name="searchAppointmentSlots" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentSlotsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentSlotsRequest"></wsdl:input>
      <wsdl:output message="tns:searchAppointmentSlotsResponse" name="searchAppointmentSlotsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentSlotsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentSlotsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentSlots/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchSales">
      <wsdl:input message="tns:searchSales" name="searchSales" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchSalesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchSalesRequest"></wsdl:input>
      <wsdl:output message="tns:searchSalesResponse" name="searchSalesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchSalesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchSalesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchSales/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientsLimited">
      <wsdl:input message="tns:searchPatientsLimited" name="searchPatientsLimited" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsLimitedRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsLimitedRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientsLimitedResponse" name="searchPatientsLimitedResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsLimitedResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsLimitedResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsLimited/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updateOrderStatus">
      <wsdl:input message="tns:updateOrderStatus" name="updateOrderStatus" wsam:Action="http://ws.partner.revolutionehr.com/partner/updateOrderStatusRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updateOrderStatusRequest"></wsdl:input>
      <wsdl:output message="tns:updateOrderStatusResponse" name="updateOrderStatusResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/updateOrderStatusResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updateOrderStatusResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/updateOrderStatus/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="rescheduleAppointmentFromDetails">
      <wsdl:input message="tns:rescheduleAppointmentFromDetails" name="rescheduleAppointmentFromDetails" wsam:Action="http://ws.partner.revolutionehr.com/partner/rescheduleAppointmentFromDetailsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/rescheduleAppointmentFromDetailsRequest"></wsdl:input>
      <wsdl:output message="tns:rescheduleAppointmentFromDetailsResponse" name="rescheduleAppointmentFromDetailsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/rescheduleAppointmentFromDetailsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/rescheduleAppointmentFromDetailsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/rescheduleAppointmentFromDetails/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTodaysInProgressEncounters">
      <wsdl:input message="tns:searchTodaysInProgressEncounters" name="searchTodaysInProgressEncounters" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTodaysInProgressEncountersRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTodaysInProgressEncountersRequest"></wsdl:input>
      <wsdl:output message="tns:searchTodaysInProgressEncountersResponse" name="searchTodaysInProgressEncountersResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTodaysInProgressEncountersResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTodaysInProgressEncountersResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTodaysInProgressEncounters/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAppointmentById">
      <wsdl:input message="tns:getAppointmentById" name="getAppointmentById" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentByIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentByIdRequest"></wsdl:input>
      <wsdl:output message="tns:getAppointmentByIdResponse" name="getAppointmentByIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentByIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentByIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentById/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchScheduleItems">
      <wsdl:input message="tns:searchScheduleItems" name="searchScheduleItems" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchScheduleItemsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchScheduleItemsRequest"></wsdl:input>
      <wsdl:output message="tns:searchScheduleItemsResponse" name="searchScheduleItemsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchScheduleItemsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchScheduleItemsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchScheduleItems/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updatePatientCommunicationPreferences">
      <wsdl:input message="tns:updatePatientCommunicationPreferences" name="updatePatientCommunicationPreferences" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientCommunicationPreferencesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updatePatientCommunicationPreferencesRequest"></wsdl:input>
      <wsdl:output message="tns:updatePatientCommunicationPreferencesResponse" name="updatePatientCommunicationPreferencesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientCommunicationPreferencesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updatePatientCommunicationPreferencesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientCommunicationPreferences/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEmployees">
      <wsdl:input message="tns:getEmployees" name="getEmployees" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEmployeesRequest"></wsdl:input>
      <wsdl:output message="tns:getEmployeesResponse" name="getEmployeesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEmployeesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployees/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatients">
      <wsdl:input message="tns:searchPatients" name="searchPatients" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientsResponse" name="searchPatientsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatients/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientById">
      <wsdl:input message="tns:getPatientById" name="getPatientById" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientByIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientByIdRequest"></wsdl:input>
      <wsdl:output message="tns:getPatientByIdResponse" name="getPatientByIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientByIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientByIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientById/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="cancelAppointment">
      <wsdl:input message="tns:cancelAppointment" name="cancelAppointment" wsam:Action="http://ws.partner.revolutionehr.com/partner/cancelAppointmentRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/cancelAppointmentRequest"></wsdl:input>
      <wsdl:output message="tns:cancelAppointmentResponse" name="cancelAppointmentResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/cancelAppointmentResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/cancelAppointmentResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/cancelAppointment/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientInsuranceTypes">
      <wsdl:input message="tns:getPatientInsuranceTypes" name="getPatientInsuranceTypes" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceTypesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceTypesRequest"></wsdl:input>
      <wsdl:output message="tns:getPatientInsuranceTypesResponse" name="getPatientInsuranceTypesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceTypesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceTypesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceTypes/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTransactionsV2">
      <wsdl:input message="tns:searchTransactionsV2" name="searchTransactionsV2" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsV2Request" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsV2Request"></wsdl:input>
      <wsdl:output message="tns:searchTransactionsV2Response" name="searchTransactionsV2Response" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsV2Response" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsV2Response"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchTransactionsV2/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getProviderIdByEmployeeId">
      <wsdl:input message="tns:getProviderIdByEmployeeId" name="getProviderIdByEmployeeId" wsam:Action="http://ws.partner.revolutionehr.com/partner/getProviderIdByEmployeeIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getProviderIdByEmployeeIdRequest"></wsdl:input>
      <wsdl:output message="tns:getProviderIdByEmployeeIdResponse" name="getProviderIdByEmployeeIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getProviderIdByEmployeeIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getProviderIdByEmployeeIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getProviderIdByEmployeeId/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getKeyDatesForPatient">
      <wsdl:input message="tns:getKeyDatesForPatient" name="getKeyDatesForPatient" wsam:Action="http://ws.partner.revolutionehr.com/partner/getKeyDatesForPatientRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getKeyDatesForPatientRequest"></wsdl:input>
      <wsdl:output message="tns:getKeyDatesForPatientResponse" name="getKeyDatesForPatientResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getKeyDatesForPatientResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getKeyDatesForPatientResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getKeyDatesForPatient/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchServices">
      <wsdl:input message="tns:searchServices" name="searchServices" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchServicesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchServicesRequest"></wsdl:input>
      <wsdl:output message="tns:searchServicesResponse" name="searchServicesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchServicesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchServicesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchServices/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAccountSummaryWithInsurance">
      <wsdl:input message="tns:getAccountSummaryWithInsurance" name="getAccountSummaryWithInsurance" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAccountSummaryWithInsuranceRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAccountSummaryWithInsuranceRequest"></wsdl:input>
      <wsdl:output message="tns:getAccountSummaryWithInsuranceResponse" name="getAccountSummaryWithInsuranceResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAccountSummaryWithInsuranceResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAccountSummaryWithInsuranceResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAccountSummaryWithInsurance/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchClaims">
      <wsdl:input message="tns:searchClaims" name="searchClaims" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchClaimsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchClaimsRequest"></wsdl:input>
      <wsdl:output message="tns:searchClaimsResponse" name="searchClaimsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchClaimsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchClaimsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchClaims/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchOrders">
      <wsdl:input message="tns:searchOrders" name="searchOrders" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchOrdersRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchOrdersRequest"></wsdl:input>
      <wsdl:output message="tns:searchOrdersResponse" name="searchOrdersResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchOrdersResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchOrdersResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchOrders/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchProducts">
      <wsdl:input message="tns:searchProducts" name="searchProducts" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchProductsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchProductsRequest"></wsdl:input>
      <wsdl:output message="tns:searchProductsResponse" name="searchProductsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchProductsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchProductsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchProducts/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAppointmentDetailById">
      <wsdl:input message="tns:getAppointmentDetailById" name="getAppointmentDetailById" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentDetailByIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentDetailByIdRequest"></wsdl:input>
      <wsdl:output message="tns:getAppointmentDetailByIdResponse" name="getAppointmentDetailByIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentDetailByIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentDetailByIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAppointmentDetailById/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientSchedulingPreferences">
      <wsdl:input message="tns:getPatientSchedulingPreferences" name="getPatientSchedulingPreferences" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientSchedulingPreferencesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientSchedulingPreferencesRequest"></wsdl:input>
      <wsdl:output message="tns:getPatientSchedulingPreferencesResponse" name="getPatientSchedulingPreferencesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientSchedulingPreferencesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientSchedulingPreferencesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientSchedulingPreferences/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchAppointments">
      <wsdl:input message="tns:searchAppointments" name="searchAppointments" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsRequest"></wsdl:input>
      <wsdl:output message="tns:searchAppointmentsResponse" name="searchAppointmentsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointments/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getOrderDetailById">
      <wsdl:input message="tns:getOrderDetailById" name="getOrderDetailById" wsam:Action="http://ws.partner.revolutionehr.com/partner/getOrderDetailByIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getOrderDetailByIdRequest"></wsdl:input>
      <wsdl:output message="tns:getOrderDetailByIdResponse" name="getOrderDetailByIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getOrderDetailByIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getOrderDetailByIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getOrderDetailById/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="echo">
      <wsdl:input message="tns:echo" name="echo" wsam:Action="http://ws.partner.revolutionehr.com/partner/echoRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/echoRequest"></wsdl:input>
      <wsdl:output message="tns:echoResponse" name="echoResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/echoResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/echoResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/echo/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchRefractions">
      <wsdl:input message="tns:searchRefractions" name="searchRefractions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchRefractionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchRefractionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchRefractionsResponse" name="searchRefractionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchRefractionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchRefractionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchRefractions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPayments">
      <wsdl:input message="tns:searchPayments" name="searchPayments" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsRequest"></wsdl:input>
      <wsdl:output message="tns:searchPaymentsResponse" name="searchPaymentsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPayments/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientInsuranceInfo">
      <wsdl:input message="tns:getPatientInsuranceInfo" name="getPatientInsuranceInfo" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceInfoRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceInfoRequest"></wsdl:input>
      <wsdl:output message="tns:getPatientInsuranceInfoResponse" name="getPatientInsuranceInfoResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceInfoResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceInfoResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsuranceInfo/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchAppointmentsWithDetail">
      <wsdl:input message="tns:searchAppointmentsWithDetail" name="searchAppointmentsWithDetail" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsWithDetailRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsWithDetailRequest"></wsdl:input>
      <wsdl:output message="tns:searchAppointmentsWithDetailResponse" name="searchAppointmentsWithDetailResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsWithDetailResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsWithDetailResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchAppointmentsWithDetail/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAllEmployees">
      <wsdl:input message="tns:getAllEmployees" name="getAllEmployees" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAllEmployeesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAllEmployeesRequest"></wsdl:input>
      <wsdl:output message="tns:getAllEmployeesResponse" name="getAllEmployeesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAllEmployeesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getAllEmployeesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getAllEmployees/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchOrderDetail">
      <wsdl:input message="tns:searchOrderDetail" name="searchOrderDetail" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchOrderDetailRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchOrderDetailRequest"></wsdl:input>
      <wsdl:output message="tns:searchOrderDetailResponse" name="searchOrderDetailResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchOrderDetailResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchOrderDetailResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchOrderDetail/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientBalances">
      <wsdl:input message="tns:searchPatientBalances" name="searchPatientBalances" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientBalancesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientBalancesRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientBalancesResponse" name="searchPatientBalancesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientBalancesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientBalancesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientBalances/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="readinessCheck">
      <wsdl:input message="tns:readinessCheck" name="readinessCheck" wsam:Action="http://ws.partner.revolutionehr.com/partner/readinessCheckRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/readinessCheckRequest"></wsdl:input>
      <wsdl:output message="tns:readinessCheckResponse" name="readinessCheckResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/readinessCheckResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/readinessCheckResponse"></wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="searchEyeglassPrescriptions">
      <wsdl:input message="tns:searchEyeglassPrescriptions" name="searchEyeglassPrescriptions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchEyeglassPrescriptionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchEyeglassPrescriptionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchEyeglassPrescriptionsResponse" name="searchEyeglassPrescriptionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchEyeglassPrescriptionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchEyeglassPrescriptionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchEyeglassPrescriptions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEmployeeOffices">
      <wsdl:input message="tns:getEmployeeOffices" name="getEmployeeOffices" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeOfficesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeOfficesRequest"></wsdl:input>
      <wsdl:output message="tns:getEmployeeOfficesResponse" name="getEmployeeOfficesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeOfficesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeOfficesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEmployeeOffices/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="addPatient">
      <wsdl:input message="tns:addPatient" name="addPatient" wsam:Action="http://ws.partner.revolutionehr.com/partner/addPatientRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/addPatientRequest"></wsdl:input>
      <wsdl:output message="tns:addPatientResponse" name="addPatientResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/addPatientResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/addPatientResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/addPatient/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientPhotoContent">
      <wsdl:input message="tns:getPatientPhotoContent" name="getPatientPhotoContent" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientPhotoContentRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientPhotoContentRequest"></wsdl:input>
      <wsdl:output message="tns:getPatientPhotoContentResponse" name="getPatientPhotoContentResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientPhotoContentResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientPhotoContentResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientPhotoContent/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchExternalMedicationPrescriptions">
      <wsdl:input message="tns:searchExternalMedicationPrescriptions" name="searchExternalMedicationPrescriptions" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchExternalMedicationPrescriptionsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchExternalMedicationPrescriptionsRequest"></wsdl:input>
      <wsdl:output message="tns:searchExternalMedicationPrescriptionsResponse" name="searchExternalMedicationPrescriptionsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchExternalMedicationPrescriptionsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchExternalMedicationPrescriptionsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchExternalMedicationPrescriptions/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchKeyDatesDetail">
      <wsdl:input message="tns:searchKeyDatesDetail" name="searchKeyDatesDetail" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesDetailRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesDetailRequest"></wsdl:input>
      <wsdl:output message="tns:searchKeyDatesDetailResponse" name="searchKeyDatesDetailResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesDetailResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesDetailResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchKeyDatesDetail/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPaymentsWithLedgerPostings">
      <wsdl:input message="tns:searchPaymentsWithLedgerPostings" name="searchPaymentsWithLedgerPostings" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsWithLedgerPostingsRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsWithLedgerPostingsRequest"></wsdl:input>
      <wsdl:output message="tns:searchPaymentsWithLedgerPostingsResponse" name="searchPaymentsWithLedgerPostingsResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsWithLedgerPostingsResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsWithLedgerPostingsResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPaymentsWithLedgerPostings/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientInsurancePriorities">
      <wsdl:input message="tns:getPatientInsurancePriorities" name="getPatientInsurancePriorities" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsurancePrioritiesRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsurancePrioritiesRequest"></wsdl:input>
      <wsdl:output message="tns:getPatientInsurancePrioritiesResponse" name="getPatientInsurancePrioritiesResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsurancePrioritiesResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsurancePrioritiesResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getPatientInsurancePriorities/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="verifyPatientUserNameAvailable">
      <wsdl:input message="tns:verifyPatientUserNameAvailable" name="verifyPatientUserNameAvailable" wsam:Action="http://ws.partner.revolutionehr.com/partner/verifyPatientUserNameAvailableRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/verifyPatientUserNameAvailableRequest"></wsdl:input>
      <wsdl:output message="tns:verifyPatientUserNameAvailableResponse" name="verifyPatientUserNameAvailableResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/verifyPatientUserNameAvailableResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/verifyPatientUserNameAvailableResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/verifyPatientUserNameAvailable/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientInsuranceInfo">
      <wsdl:input message="tns:searchPatientInsuranceInfo" name="searchPatientInsuranceInfo" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientInsuranceInfoRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientInsuranceInfoRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientInsuranceInfoResponse" name="searchPatientInsuranceInfoResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientInsuranceInfoResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientInsuranceInfoResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientInsuranceInfo/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getProviders">
      <wsdl:input message="tns:getProviders" name="getProviders" wsam:Action="http://ws.partner.revolutionehr.com/partner/getProvidersRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getProvidersRequest"></wsdl:input>
      <wsdl:output message="tns:getProvidersResponse" name="getProvidersResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getProvidersResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getProvidersResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getProviders/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEncounterById">
      <wsdl:input message="tns:getEncounterById" name="getEncounterById" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEncounterByIdRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEncounterByIdRequest"></wsdl:input>
      <wsdl:output message="tns:getEncounterByIdResponse" name="getEncounterByIdResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEncounterByIdResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/getEncounterByIdResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/getEncounterById/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updatePatientLogin">
      <wsdl:input message="tns:updatePatientLogin" name="updatePatientLogin" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientLoginRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updatePatientLoginRequest"></wsdl:input>
      <wsdl:output message="tns:updatePatientLoginResponse" name="updatePatientLoginResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientLoginResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/updatePatientLoginResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/updatePatientLogin/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="confirmAppointment">
      <wsdl:input message="tns:confirmAppointment" name="confirmAppointment" wsam:Action="http://ws.partner.revolutionehr.com/partner/confirmAppointmentRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/confirmAppointmentRequest"></wsdl:input>
      <wsdl:output message="tns:confirmAppointmentResponse" name="confirmAppointmentResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/confirmAppointmentResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/confirmAppointmentResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/confirmAppointment/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientsWithReferral">
      <wsdl:input message="tns:searchPatientsWithReferral" name="searchPatientsWithReferral" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsWithReferralRequest" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsWithReferralRequest"></wsdl:input>
      <wsdl:output message="tns:searchPatientsWithReferralResponse" name="searchPatientsWithReferralResponse" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsWithReferralResponse" wsaw:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsWithReferralResponse"></wsdl:output>
      <wsdl:fault message="tns:WebServiceException" name="WebServiceException" wsam:Action="http://ws.partner.revolutionehr.com/partner/searchPatientsWithReferral/Fault/WebServiceException"></wsdl:fault>
    </wsdl:operation>
  </wsdl:portType>
  <wsdl:binding name="PartnerServiceSoapBinding" type="tns:partner">
    <soap12:binding style="document" transport="http://schemas.xmlsoap.org/soap/http"/>
    <wsaw:UsingAddressing xmlns:wsdl="http://schemas.xmlsoap.org/wsdl/" xmlns:wsaw="http://www.w3.org/2006/05/addressing/wsdl" wsdl:required="false"/>
    <wsp:PolicyReference URI="#PartnerServiceSoapBinding_WSAM_Addressing_Policy"/>
    <wsdl:operation name="searchPaymentItems">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPaymentItems">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPaymentItemsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="uploadPatientFilesToFolder">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="uploadPatientFilesToFolder">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="uploadPatientFilesToFolderResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="deactivatePatient">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="deactivatePatient">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="deactivatePatientResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getInvoiceNotes">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getInvoiceNotes">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getInvoiceNotesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="setPatientNotified">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="setPatientNotified">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="setPatientNotifiedResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getRecallById">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getRecallById">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getRecallByIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchContactLensPrescriptions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchContactLensPrescriptions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchContactLensPrescriptionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="activatePatient">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="activatePatient">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="activatePatientResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updatePatient">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="updatePatient">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="updatePatientResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientDiagnoses">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientDiagnoses">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientDiagnosesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientTransactions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientTransactions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientTransactionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchDeletedRecalls">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchDeletedRecalls">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchDeletedRecallsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTransactions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchTransactions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchTransactionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTransactionsWithDiagnoses">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchTransactionsWithDiagnoses">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchTransactionsWithDiagnosesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getServerTime">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getServerTime">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getServerTimeResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchKeyDates">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchKeyDates">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchKeyDatesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPaymentItemsWithLedgerPostings">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPaymentItemsWithLedgerPostings">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPaymentItemsWithLedgerPostingsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="createAppointmentFromSlot">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="createAppointmentFromSlot">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="createAppointmentFromSlotResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEmployeeIdByProviderId">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getEmployeeIdByProviderId">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getEmployeeIdByProviderIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="deceasePatient">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="deceasePatient">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="deceasePatientResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchRecalls">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchRecalls">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchRecallsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchMedicationPrescriptions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchMedicationPrescriptions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchMedicationPrescriptionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAllProviders">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getAllProviders">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getAllProvidersResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getOffices">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getOffices">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getOfficesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientPhotos">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientPhotos">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientPhotosResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="createAppointmentFromDetails">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="createAppointmentFromDetails">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="createAppointmentFromDetailsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchInvoicePayments">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchInvoicePayments">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchInvoicePaymentsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getInsuranceCompanies">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getInsuranceCompanies">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getInsuranceCompaniesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchEncounters">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchEncounters">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchEncountersResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getApptTypes">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getApptTypes">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getApptTypesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchAppointmentSlots">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchAppointmentSlots">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchAppointmentSlotsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchSales">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchSales">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchSalesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientsLimited">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientsLimited">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientsLimitedResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updateOrderStatus">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="updateOrderStatus">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="updateOrderStatusResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="rescheduleAppointmentFromDetails">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="rescheduleAppointmentFromDetails">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="rescheduleAppointmentFromDetailsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTodaysInProgressEncounters">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchTodaysInProgressEncounters">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchTodaysInProgressEncountersResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAppointmentById">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getAppointmentById">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getAppointmentByIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchScheduleItems">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchScheduleItems">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchScheduleItemsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updatePatientCommunicationPreferences">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="updatePatientCommunicationPreferences">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="updatePatientCommunicationPreferencesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEmployees">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getEmployees">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getEmployeesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatients">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatients">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientById">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getPatientById">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getPatientByIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="cancelAppointment">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="cancelAppointment">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="cancelAppointmentResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientInsuranceTypes">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getPatientInsuranceTypes">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getPatientInsuranceTypesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchTransactionsV2">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchTransactionsV2">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchTransactionsV2Response">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getProviderIdByEmployeeId">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getProviderIdByEmployeeId">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getProviderIdByEmployeeIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getKeyDatesForPatient">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getKeyDatesForPatient">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getKeyDatesForPatientResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchServices">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchServices">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchServicesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAccountSummaryWithInsurance">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getAccountSummaryWithInsurance">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getAccountSummaryWithInsuranceResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchClaims">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchClaims">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchClaimsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchOrders">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchOrders">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchOrdersResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchProducts">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchProducts">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchProductsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAppointmentDetailById">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getAppointmentDetailById">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getAppointmentDetailByIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientSchedulingPreferences">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getPatientSchedulingPreferences">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getPatientSchedulingPreferencesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchAppointments">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchAppointments">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchAppointmentsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getOrderDetailById">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getOrderDetailById">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getOrderDetailByIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="echo">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="echo">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="echoResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchRefractions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchRefractions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchRefractionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPayments">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPayments">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPaymentsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientInsuranceInfo">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getPatientInsuranceInfo">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getPatientInsuranceInfoResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchAppointmentsWithDetail">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchAppointmentsWithDetail">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchAppointmentsWithDetailResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getAllEmployees">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getAllEmployees">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getAllEmployeesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchOrderDetail">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchOrderDetail">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchOrderDetailResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientBalances">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientBalances">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientBalancesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="readinessCheck">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="readinessCheck">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="readinessCheckResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="searchEyeglassPrescriptions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchEyeglassPrescriptions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchEyeglassPrescriptionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEmployeeOffices">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getEmployeeOffices">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getEmployeeOfficesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="addPatient">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="addPatient">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="addPatientResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientPhotoContent">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getPatientPhotoContent">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getPatientPhotoContentResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchExternalMedicationPrescriptions">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchExternalMedicationPrescriptions">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchExternalMedicationPrescriptionsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchKeyDatesDetail">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchKeyDatesDetail">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchKeyDatesDetailResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPaymentsWithLedgerPostings">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPaymentsWithLedgerPostings">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPaymentsWithLedgerPostingsResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getPatientInsurancePriorities">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getPatientInsurancePriorities">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getPatientInsurancePrioritiesResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="verifyPatientUserNameAvailable">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="verifyPatientUserNameAvailable">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="verifyPatientUserNameAvailableResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientInsuranceInfo">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientInsuranceInfo">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientInsuranceInfoResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getProviders">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getProviders">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getProvidersResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="getEncounterById">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="getEncounterById">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="getEncounterByIdResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="updatePatientLogin">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="updatePatientLogin">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="updatePatientLoginResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="confirmAppointment">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="confirmAppointment">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="confirmAppointmentResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
    <wsdl:operation name="searchPatientsWithReferral">
      <soap12:operation soapAction="" style="document"/>
      <wsdl:input name="searchPatientsWithReferral">
        <soap12:body use="literal"/>
      </wsdl:input>
      <wsdl:output name="searchPatientsWithReferralResponse">
        <soap12:body use="literal"/>
      </wsdl:output>
      <wsdl:fault name="WebServiceException">
        <soap12:fault name="WebServiceException" use="literal"/>
      </wsdl:fault>
    </wsdl:operation>
  </wsdl:binding>
  <wsdl:service name="PartnerService">
    <wsdl:port binding="tns:PartnerServiceSoapBinding" name="PartnerPort">
      <soap12:address location="https://services.revolutionehr.com/ws/services/partner"/>
    </wsdl:port>
  </wsdl:service>
  <wsp:Policy xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd" wsu:Id="PartnerServiceSoapBinding_WSAM_Addressing_Policy">
    <wsam:Addressing wsp:Optional="true">
      <wsp:Policy/>
    </wsam:Addressing>
  </wsp:Policy>
</wsdl:definitions>
```
