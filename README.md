# PhoneBook

Please run the following script in SQL:

CREATE DATABASE [PhoneBook]
GO

USE [PhoneBook]
GO
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
SET ANSI_PADDING ON
GO
CREATE TABLE [dbo].[Directory](
	[Id] [int] IDENTITY(1,1) NOT NULL,
	[Name] [varchar](100) NOT NULL,
	[Phone_Number] [varchar](100) NOT NULL,
 CONSTRAINT [PK_Directory] PRIMARY KEY CLUSTERED 
(
	[Id] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY]
GO

SET ANSI_PADDING OFF
GO

Insert into [PhoneBook].[dbo].[Directory] values ('Sutasha Dookhi','0645-127890')
Insert into [PhoneBook].[dbo].[Directory] values ('Nelie Mostert','0644-195890')
Insert into [PhoneBook].[dbo].[Directory] values ('Valieta Barnard','0825-337890')
Insert into [PhoneBook].[dbo].[Directory] values ('Damian Cholewka','0735-146890')

GO
