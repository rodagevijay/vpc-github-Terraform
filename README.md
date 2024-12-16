# vpc-github-Terraform
creating vpc
USE [MLLITAMS]
GO

/****** Object:  Table [dbo].[NewITAssetDetails_Desktop]    Script Date: 16/12/24 18:10:03 ******/
SET ANSI_NULLS ON
GO

SET QUOTED_IDENTIFIER ON
GO

CREATE TABLE [dbo].[NewITAssetDetails_Desktop](
	[Asset_ID] [int] IDENTITY(1,1) NOT NULL,
	[Category] [nvarchar](200) NULL,
	[Asset_No] [nvarchar](200) NULL,
	[Host_Name] [nvarchar](200) NULL,
	[Location] [nvarchar](50) NULL,
	[Bar_Code] [nvarchar](200) NULL,
	[Model] [nvarchar](200) NULL,
	[Manufacturer] [nvarchar](200) NULL,
	[Part_No] [nvarchar](200) NULL,
	[Serial_No] [nvarchar](200) NULL,
	[Processor] [nvarchar](200) NULL,
	[RAM] [nvarchar](200) NULL,
	[HDD] [nvarchar](200) NULL,
	[Config] [nvarchar](max) NULL,
	[IP_Address] [nvarchar](200) NULL,
	[Monitor_Type] [nvarchar](200) NULL,
	[Make] [nvarchar](200) NULL,
	[Size] [nvarchar](200) NULL,
	[Keyboard] [nvarchar](200) NULL,
	[Mouse] [nvarchar](200) NULL,
	[GxP_Applicable] [nvarchar](200) NULL,
	[System_Revalidation_Date] [date] NULL,
	[Usage_Type] [nvarchar](200) NULL,
	[InstName] [nvarchar](200) NULL,
	[InstType] [nvarchar](200) NULL,
	[Version] [nvarchar](200) NULL,
	[Software] [nvarchar](200) NULL,
	[EmpNo] [nvarchar](200) NULL,
	[OperatingSystem] [nvarchar](200) NULL,
	[Sw_Version] [nvarchar](200) NULL,
	[ProductKey] [nvarchar](200) NULL,
	[AssetState] [nvarchar](200) NULL,
	[NatureofActivities] [nvarchar](max) NULL,
	[PONumber] [nvarchar](200) NULL,
	[PODate] [date] NULL,
	[InvoiceNumber] [nvarchar](200) NULL,
	[InvoiceDate] [date] NULL,
	[SupplierName] [nvarchar](200) NULL,
	[Value] [nvarchar](200) NULL,
	[WarrantyExpiration] [date] NULL,
	[PreventiveMaintenace] [date] NULL,
	[InstallationDate] [date] NULL,
	[InstallationType] [nvarchar](200) NULL,
	[Created_by] [nvarchar](200) NULL,
	[Created_date] [datetime] NULL,
	[Modified_by] [nvarchar](200) NULL,
	[Modified_date] [datetime] NULL,
	[Other_Software_Name] [nvarchar](200) NULL,
	[Other_version] [nvarchar](200) NULL,
	[Other_product_key] [nvarchar](200) NULL,
	[Other_Expiry_on] [date] NULL,
	[Remarks] [nvarchar](max) NULL,
	[Date_of_Issue] [date] NULL,
	[Ppm] [nvarchar](200) NULL,
	[Machine_Life] [nvarchar](200) NULL,
	[Cpp] [nvarchar](200) NULL,
	[Asset_Type] [nvarchar](50) NULL,
	[EmpAd] [nvarchar](50) NULL,
	[size_type] [nvarchar](50) NULL,
	[ram_size] [nvarchar](50) NULL,
	[com_dept] [nvarchar](50) NULL,
	[com_floor] [nvarchar](50) NULL,
	[replacement_type] [nvarchar](200) NULL,
	[viewStatusApprover] [nvarchar](50) NULL,
	[statusApprovedDate] [datetime] NULL,
	[reportViewStatus] [int] NULL,
 CONSTRAINT [PK_NewITAssetDetails_Desktop] PRIMARY KEY CLUSTERED 
(
	[Asset_ID] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY] TEXTIMAGE_ON [PRIMARY]
GO

ALTER TABLE [dbo].[NewITAssetDetails_Desktop] ADD  CONSTRAINT [D_reportViewStatus]  DEFAULT ((0)) FOR [reportViewStatus]
GO


