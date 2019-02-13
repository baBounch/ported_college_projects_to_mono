MAINPROGRAM=Program
EXECUTABLE=${MAINPROGRAM}.exe
MAINCS=${MAINPROGRAM}.cs
CSFILES=${MAINCS} frmInvoiceTotal.cs frmInvoiceTotal.Designer.cs
RESOURCES=-r:System.Windows.Forms.dll -r:System.Data.dll -r:System.Drawing.dll
PARAMS=${CSFILES} ${RESOURCES}

:all mono

mono: ${MAINCS}
	mcs ${PARAMS}

dotnet: ${MAINCS}
	csc ${PARAMS}

clean:
	rm ${EXECUTABLE} -r -f
